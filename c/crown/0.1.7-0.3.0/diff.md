# Comparing `tmp/crown-0.1.7.tar.gz` & `tmp/crown-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/crown-0.1.7.tar", last modified: Mon Feb 28 03:35:15 2022, max compression
+gzip compressed data, was "crown-0.3.0.tar", last modified: Tue Jun 27 03:34:55 2023, max compression
```

## Comparing `crown-0.1.7.tar` & `crown-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 machine    (501) staff       (20)        0 2022-02-28 03:35:15.370565 crown-0.1.7/
--rw-r--r--   0 machine    (501) staff       (20)    26516 2022-02-28 03:35:15.369961 crown-0.1.7/PKG-INFO
--rw-r--r--   0 machine    (501) staff       (20)    22010 2022-02-20 04:38:24.000000 crown-0.1.7/README.rst
-drwxr-xr-x   0 machine    (501) staff       (20)        0 2022-02-28 03:35:15.366742 crown-0.1.7/crown/
--rw-r--r--   0 machine    (501) staff       (20)      395 2020-11-29 05:27:00.000000 crown-0.1.7/crown/__init__.py
--rw-r--r--   0 machine    (501) staff       (20)     1718 2020-12-02 02:00:56.000000 crown-0.1.7/crown/common.py
--rw-r--r--   0 machine    (501) staff       (20)    18044 2022-02-20 04:14:59.000000 crown-0.1.7/crown/crown.py
--rw-r--r--   0 machine    (501) staff       (20)     7025 2022-02-19 08:51:02.000000 crown-0.1.7/crown/database.py
--rw-r--r--   0 machine    (501) staff       (20)     3333 2022-02-28 02:38:59.000000 crown-0.1.7/crown/eng_taosrestful.py
--rw-r--r--   0 machine    (501) staff       (20)     7791 2022-02-19 08:51:02.000000 crown-0.1.7/crown/field.py
--rw-r--r--   0 machine    (501) staff       (20)    27039 2022-02-20 04:34:44.000000 crown-0.1.7/crown/query.py
-drwxr-xr-x   0 machine    (501) staff       (20)        0 2022-02-28 03:35:15.369120 crown-0.1.7/crown.egg-info/
--rw-r--r--   0 machine    (501) staff       (20)    26516 2022-02-28 03:35:15.000000 crown-0.1.7/crown.egg-info/PKG-INFO
--rw-r--r--   0 machine    (501) staff       (20)      285 2022-02-28 03:35:15.000000 crown-0.1.7/crown.egg-info/SOURCES.txt
--rw-r--r--   0 machine    (501) staff       (20)        1 2022-02-28 03:35:15.000000 crown-0.1.7/crown.egg-info/dependency_links.txt
--rw-r--r--   0 machine    (501) staff       (20)       17 2022-02-28 03:35:15.000000 crown-0.1.7/crown.egg-info/requires.txt
--rw-r--r--   0 machine    (501) staff       (20)        6 2022-02-28 03:35:15.000000 crown-0.1.7/crown.egg-info/top_level.txt
--rw-r--r--   0 machine    (501) staff       (20)       38 2022-02-28 03:35:15.370771 crown-0.1.7/setup.cfg
--rw-r--r--   0 machine    (501) staff       (20)     1099 2022-02-28 03:04:42.000000 crown-0.1.7/setup.py
+drwxr-xr-x   0 machine    (501) staff       (20)        0 2023-06-27 03:34:55.979344 crown-0.3.0/
+-rw-r--r--   0 machine    (501) staff       (20)     1064 2023-06-27 00:25:34.000000 crown-0.3.0/LICENSE
+-rw-r--r--   0 machine    (501) staff       (20)    22502 2023-06-27 03:34:55.979198 crown-0.3.0/PKG-INFO
+-rw-r--r--   0 machine    (501) staff       (20)    22062 2023-06-27 03:15:14.000000 crown-0.3.0/README.rst
+drwxr-xr-x   0 machine    (501) staff       (20)        0 2023-06-27 03:34:55.978256 crown-0.3.0/crown/
+-rw-r--r--   0 machine    (501) staff       (20)      395 2023-06-27 03:15:23.000000 crown-0.3.0/crown/__init__.py
+-rw-r--r--   0 machine    (501) staff       (20)     1718 2023-06-27 01:43:26.000000 crown-0.3.0/crown/common.py
+-rw-r--r--   0 machine    (501) staff       (20)    18278 2023-06-27 02:28:59.000000 crown-0.3.0/crown/crown.py
+-rw-r--r--   0 machine    (501) staff       (20)     7227 2023-06-27 02:39:01.000000 crown-0.3.0/crown/database.py
+-rw-r--r--   0 machine    (501) staff       (20)     3333 2023-06-27 01:44:38.000000 crown-0.3.0/crown/eng_taosrestful.py
+-rw-r--r--   0 machine    (501) staff       (20)     3469 2023-06-27 01:44:45.000000 crown-0.3.0/crown/eng_taosrestful3.py
+-rw-r--r--   0 machine    (501) staff       (20)     7895 2023-06-27 02:27:17.000000 crown-0.3.0/crown/field.py
+-rw-r--r--   0 machine    (501) staff       (20)    27152 2023-06-27 02:58:52.000000 crown-0.3.0/crown/query.py
+drwxr-xr-x   0 machine    (501) staff       (20)        0 2023-06-27 03:34:55.978992 crown-0.3.0/crown.egg-info/
+-rw-r--r--   0 machine    (501) staff       (20)    22502 2023-06-27 03:34:55.000000 crown-0.3.0/crown.egg-info/PKG-INFO
+-rw-r--r--   0 machine    (501) staff       (20)      319 2023-06-27 03:34:55.000000 crown-0.3.0/crown.egg-info/SOURCES.txt
+-rw-r--r--   0 machine    (501) staff       (20)        1 2023-06-27 03:34:55.000000 crown-0.3.0/crown.egg-info/dependency_links.txt
+-rw-r--r--   0 machine    (501) staff       (20)       17 2023-06-27 03:34:55.000000 crown-0.3.0/crown.egg-info/requires.txt
+-rw-r--r--   0 machine    (501) staff       (20)        6 2023-06-27 03:34:55.000000 crown-0.3.0/crown.egg-info/top_level.txt
+-rw-r--r--   0 machine    (501) staff       (20)       38 2023-06-27 03:34:55.979385 crown-0.3.0/setup.cfg
+-rw-r--r--   0 machine    (501) staff       (20)     1099 2023-06-27 03:23:04.000000 crown-0.3.0/setup.py
```

### Comparing `crown-0.1.7/PKG-INFO` & `crown-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,518 +1,518 @@
 Metadata-Version: 2.1
 Name: crown
-Version: 0.1.7
+Version: 0.3.0
 Summary: crown is a simple and small ORM for Time Series Database (TSDB) tdengine(taos), making it easy to learn and intuitive to use.
 Home-page: https://github.com/machine-w/crown
 Author: machine-w
 Author-email: steve2008.ma@gmail.com
-License: UNKNOWN
-Description: crown
-        ======
-        
-        crown 是一个轻量级的针对时序数据（TSDB）TDengine的ORM库。 
-        
-        * 需要python 3.0版本以上
-        * 在tdengine 2.0.8版本测试通过
-        * 解决mac操作系统下没有原生python连接器的问题
-        * 极大的降低了python程序员使用TDengine技术门槛
-        * 可以方便的将数据转换到numpy与pandas
-        * 目前使用TDengine的restful接口连接数据库，以后将提供原生接口引擎可供选择（目前原生接口无法在mac系统上使用）
-        
-        安装
-        ----------------------
-        
-        大多数情况下，可以通过pip,轻松安装最新版本：
-        
-        .. code-block:: console
-        
-            pip install crown
-        
-        
-        还可以通过git安装，项目地址： https://github.com/machine-w/crown
-        
-        使用方法:
-        
-        .. code-block:: console
-        
-            git clone https://github.com/machine-w/crown.git
-            cd crowm
-            python setup.py install
-        
-        
-        使用文档
-        ------------------------
-        
-        建立数据库与删除数据库:
-        
-        .. code-block:: python
-        
-            from crown import *
-        
-            DATABASENAME = 'taos_test'
-            HOST = 'localhost'
-            PORT = 6041
-            # 默认端口 6041，默认用户名：root,默认密码：taosdata
-            db = TdEngineDatabase(DATABASENAME,host=HOST) #新建数据库对象
-            # db.connect()  # 尝试连接数据库，如果库不存在，则自动建库。
-            # print(db.databases) #连接数据库db对象后会自动获取全部数据库信息，以字典的形式保存在属性databases中。
-            # 如不使用默认值，可以如下传入参数
-            # db = TdEngineDatabase(DATABASENAME,host=HOST,port=PORT,user='yourusername',passwd='yourpassword')
-            db.create_database(safe=True)  #建库指令。 （safe：如果库存在，则跳过建库指令。）
-            # db.create_database(safe=True,keep= 100,comp=0,replica=1,quorum=2,blocks=115) #可选字段：建库时配置数据库参数，具体字段含义请参考tdengine文档。
-            db.drop_database(safe=True) #删库指令 （safe：如果库不存在，则跳过删库指令。）
-        
-        修改数据库参数:
-        
-        .. code-block:: python
-        
-            db.alter_database(keep= 120,comp=1,replica=1,quorum=1,blocks=156) #同建库可选字段。
-        
-        执行sql语句:
-        
-        .. code-block:: python
-        
-            #可以通过数据库对象直接执行sql语句，语句规则与TDengine restful接口要求一致。
-            res = db.raw_sql('select c1,c2 from taos_test.member1')
-            print(res,res.head,res.rowcount) #返回的对象为二维数据。res.head属性为数组对象，保存每一行数据的代表的列名。res.rowcount属性保存返回行数。
-            # res: [[1.2,2.2],[1.3,2.1],[1.5,2.0],[1.6,2.1]]
-            # res.head: ['c1','c2']
-            # res.rowcount: 4
-        
-        打印执行的sql语句:
-        
-        .. code-block:: python
-        
-            Meter1.select().one()
-            print(db.curSql) #可以通过db对象的curSql属性获取当前执行的原始sql语句
-        
-        模型定义:
-        
-        .. code-block:: python
-        
-            from crown import *
-        
-            DATABASENAME = 'taos_test'
-            HOST = 'localhost'
-            db = TdEngineDatabase(DATABASENAME,host=HOST) #新建数据库对象
-            db.connect()  #尝试连接数据库，如果库不存在，则自动建库。
-            # print(db.databases) #连接数据库db对象后会自动获取全部数据库信息，以字典的形式保存在属性databases中。
-        
-            # 表模型类继承自Model类，每个模型类对应数据库中的一张表，模型类中定义的每个Field，对应表中的一列
-            class Meter1(Model):
-                cur = FloatField(db_column='c1')
-                curInt = IntegerField(db_column='c2')
-                curDouble = DoubleField(db_column='c3')
-                desc = BinaryField(db_column='des')
-        
-                class Meta: #Meta子类中定义模型类的配置信息
-                    database = db #指定表所使用的数据库
-                    db_table = 'meter1' #指定表名
-        
-            # 可选择的全部Field类型如下，类型与Tdengine支持的数据类型一一对应
-            class AllField(Model):
-                name_float = FloatField(column_name='nf1') #可选项：指定列名
-                name_double = DoubleField()
-                name_bigint = BigIntegerField()
-                name_int = IntegerField()
-                name_smallint = SmallIntegerField()
-                name_tinyint = TinyIntegerField()
-                name_nchar = NCharField(max_length=59,db_column='n1')
-                name_binary = BinaryField(max_length=3)
-                name_bool = BooleanField()
-                dd = PrimaryKeyField() # 如果定义了主键列，则使用主键列作为主键，如果没有定义，则默认“ts”为主键。
-                birthday = DateTimeField()
-                class Meta:
-                    database = db
-                    db_table = 'all_field'
-        
-        主键定义：
-        
-        .. code-block:: python
-        
-            #定义主键方式1 
-            #不定义主键，系统默认主键：“ts”
-            class TestPri(Model):
-                cur = FloatField(db_column='c1')
-                class Meta:
-                    database = db
-            res = TestPri.describe_table() #获取表结构信息
-            print(res[0][0]) # 结果: “ts”
-        
-            #定义主键方式2
-            class TestPri(Model):
-                cur = FloatField(db_column='c1')
-                timeline = PrimaryKeyField() #定义主键列，主键名设置为列名
-                class Meta:
-                    database = db
-            res = TestPri.describe_table()
-            print(res[0][0]) # 结果: “timeline”
-        
-             #定义主键方式3
-            class TestPri(Model):
-                cur = FloatField(db_column='c1')
-                class Meta:
-                    database = db
-                    primary_key = 'timeline' # Meta中定主键名称
-            res = TestPri.describe_table()
-            print(res[0][0]) # 结果: “timeline”
-            
-        
-        
-        建表、删表、检查表是否存在：
-        
-        .. code-block:: python
-        
-            Meter1.create_table(safe=True) #建表 safe：如果表存在，则跳过建表指令。命令运行成功放回True,失败raise错误
-            # db.create_table(Meter1,safe=True) #通过数据库对象建表，功能同上
-            Meter1.drop_table(safe=True) #删表 safe：如果表不存在，则跳过删表指令。命令运行成功放回True,失败raise错误
-            # db.drop_table(Meter1,safe=True) #通过数据库对象删表，功能同上
-            Meter1.table_exists() #查看表是否存在，存在返回True,不存在返回：False
-        
-        动态建表：
-        
-        除了使用定义模型类的方式建表外，还提供了动态定义字段建表的功能。
-        
-        .. code-block:: python
-        
-            #可以使用Model类的类方法dynamic_create_table方法动态建表，第一个参数为表名，然后需要指定数据库，与是否安全建表。
-            # 关键词参数可以任意多个，指定表中的字段。
-            Meter_dynamic= Model.dynamic_create_table('meterD',database=db,safe=True,test1 = FloatField(db_column='t1'),test2 = IntegerField(db_column='t2'))
-            # 函数返回的对象为Model类对象。使用方法与静态继承的模型类相同。
-            Meter_dynamic.table_exists()
-            Meter_dynamic.drop_table()
-        
-        从表名建立对应的model类：
-        
-        数据库中已有的数据库表，可以通过已知的表名建立对应的model类。
-        
-        .. code-block:: python
-        
-            nodeTable = Model.model_from_table('node_10',db) # node_10为数据表的表名
-            res = nodeTable.select().one() # 从表名新建的类和静态建立的类，使用方法完全一致
-            
-            
-        动态建立的或从数据库分析得到的model对象，可以直接使用列名作为属性名进行查询操作。
-        
-        .. code-block:: python
-        
-        
-            res = nodeTable.select(nodeTable.c1)where(nodeTable.c1 > 1).all() # 直接使用列名
-            res = nodeTable.select(nodeTable.c1)where(FloatField(db_column='c1') > 1).all() # 也可以使用field对象作为字段检索条件（多使用于列名为动态值的时候）
-            # 直接使用列名,查看结果
-            for item in res:
-                print(item.c1)
-        
-        插入数据：
-        
-        .. code-block:: python
-        
-            #方法一
-            for i in range(1,101):
-                #使用模型类实例化的每个对象对应数据表中的每一行，可以通过传入属性参数的方式给每一列赋值
-                m = Meter1(cur = 1/i,curInt=i,curDouble=1/i+10,desc='g1',ts= datetime.datetime.now() - datetime.timedelta(seconds=(102-i)))
-                #使用对象的save方法将数据存入数据库
-                m.save()
-            print(Meter1.select().count()) # 结果：100
-            #方法二
-            for i in range(1,11):
-                #也可以直接使用模型类的insert方法插入数据。
-                Meter1.insert(cur = 1/i,curInt=i,curDouble=1/i+10,desc='g1',ts= datetime.datetime.now() - datetime.timedelta(seconds=(12-i)))
-            print(Meter1.select().count()) # 结果：100
-            #如果不传入时间属性，则会以当前时刻为默认值传入
-            Meter1.insert(cur = 1/i,curInt=i,curDouble=1/i+10,desc='g1')
-            m = Meter1(cur = 1/i,curInt=i,curDouble=1/i+10,desc='g1')
-            m.save()
-        
-        查询单条数据：
-        
-        .. code-block:: python
-        
-            #获取一条数据
-            #使用select()类方法获取查询字段（参数留空表示取全部字段），然后可以链式使用one方法获取第一条数据
-            res = Meter1.select().one()
-            print(res.desc,res.curDouble,res.curInt,res.cur,res.ts)
-        
-            #select函数中可以选择要读取的字段
-            res = Meter1.select(Meter1.cur,Meter1.desc).one()
-            print(res.desc,res.curDouble,res.curInt,res.cur,res.ts)
-        
-            #select函数中可以使用Model的类方法f()和fc()获取字符串形式的属性名与列名对应Field对象
-            res = Meter1.select(Meter1.f('cur'),Meter1.fc('c3'),Meter1.desc).one()
-            print(res.desc,res.curDouble,res.curInt,res.fc('c3'),res.f('cur'),res.ts)
-        
-        查询全部数据：
-        
-        .. code-block:: python
-        
-            #获取一条数据
-            #使用select()类方法获取查询字段（参数留空表示取全部字段），然后可以链式使用all方法获取全部数据
-            res_all = Meter1.select().all()
-            for res in res_all:
-                print(res.desc,res.curDouble,res.curInt,res.cur,res.ts)
-        
-            #select函数中可以选择要读取的字段
-            res_all = Meter1.select(Meter1.cur,Meter1.desc).all()
-            for res in res_all:
-                print(res.desc,res.curDouble,res.curInt,res.cur,res.ts)
-        
-        虽然TDengine提供了很多聚合和统计函数，但是把时序数据导入numpy或pandas等数据分析组件中进行处理的情况也是很常见的操作。
-        下面介绍如何通过crown把结果数据导入numpy和pandas
-        
-        读取数据到numpy：
-        
-        .. code-block:: python
-        
-            #通过all_raw函数可以获取二维数组格式的数据查询结果。结果每列代表的标题保存在结果对象的head属性中。
-            raw_results = Meter1.select(Meter1.cur,Meter1.curInt,Meter1.curDouble).all_raw()
-            #可以很方便的将结果转换为numpy数组对象
-            np_data = np.array(raw_results)
-            print(np_data)
-            print(raw_results.head)
-        
-        读取数据到pandas：
-        
-        .. code-block:: python
-        
-            raw_results = Meter1.select().all_raw()
-            #使用以下方法，可以轻松的将数据导入pandas,并且使用时间点作为index,使用返回的数据标题作为列名。
-            pd_data = pd.DataFrame(raw_results,columns=raw_results.head).set_index('ts')
-            print(pd_data)
-        
-        选择列四则运算：
-        
-        .. code-block:: python
-        
-            #使用select()类方法获取查询字段时，可以返回某列或多列间的值加、减、乘、除、取余计算结果（+ - * / %）
-            res_all = Meter1.select((Meter1.curDouble+Meter1.cur),Meter1.ts).all()
-            for res in res_all:
-                print(res.get(Meter1.curDouble+Meter1.cur),res.ts) #返回的结果对象可以用get方法获取原始计算式结果
-        
-            #字段别名
-            res_all = Meter1.select(((Meter1.curDouble+Meter1.cur)*Meter1.curDouble).alias('new_name'),Meter1.ts).all() #给运算式起别名（不仅运算式，其他放在select函数中的任何属性都可以使用别名）
-            for res in res_all:
-                print(res.new_name,res.ts) #使用别名获取运算结果
-        
-        where查询条件：
-        
-        .. code-block:: python
-        
-            #可以在select函数后链式调用where函数进行条件限
-            one_time =datetime.datetime.now() - datetime.timedelta(hours=10)
-            ress = Meter1.select().where(Meter1.ts > one_time).all()
-            #限定条件可以使用 > < == >= <= != and or ! 等。字符类型的字段可以使用 % 作为模糊查询（相当于like）
-            # 逻辑操作符号 |: 或 &：与 ~：非。（注意：做逻辑操作符号的表达式需要用括号括起来）
-            ress = Meter1.select().where((Meter1.cur > 0) | (Meter1.desc % 'g%')).all()
-            #where函数可以接收任意多参数，每个参数为一个限定条件，参数条件之间为"与"的关系。
-            ress = Meter1.select().where(Meter1.cur > 0, Meter1.ts > one_time, Meter1.desc % '%1').all()
-        
-        分页与limit：
-        
-        .. code-block:: python
-        
-            #可以在select函数后链式调用paginate函数进行分页操作，以下例子为取第6页 每页5条数据。
-            ress_1 = Meter1.select().paginate(6,page_size=5).all()
-            ress_2 = Meter1.select().paginate(6).all() #默认page_size为20
-            #可以在select函数后链式调用limit函数和offset函数条数限制和定位操作。
-            ress_3 = Meter1.select().limit(2).offset(5).all()
-            ress_4 = Meter1.select().limit(2).all()
-        
-        排序（目前tdengine只支持主键排序）：
-        
-        .. code-block:: python
-        
-            #可以在select函数后链式调用desc或者asc函数进行时间轴的正序或者倒序查询
-            res = Meter1.select().desc().one()
-            #定义模型类的时候定义默认排序方法
-            class Meter1(Model):
-                cur = FloatField(db_column='c1')
-                curInt = IntegerField(db_column='c2')
-                curDouble = DoubleField(db_column='c3')
-                desc = BinaryField(db_column='des')
-                dd = PrimaryKeyField().desc() #可以在定义主键的时候调用field的desc或asc方法定义默认排序
-                class Meta:
-                    # order_by= ['-dd'] #也可以在元数据类中定义‘-dd’代表倒序‘dd’ 代表正序
-                    database = db
-        
-        去重 ：
-        
-        .. code-block:: python
-        
-            #可以在select函数后链式调用distinct函数对返回的数据列进行去重复操作
-            res = Meter1.select().distinct().all()
-        
-        聚合函数：
-        
-        .. code-block:: python
-        
-            #count
-            count = Meter1.select().count() #统计行数
-            print(count) # 结果： 100
-            count = Meter1.select().count(Meter1.desc) #统计指定列非空行数
-            print(count) # 结果： 90
-            #avg（sum,stddev,min,max,first,last,last_row,spread使用方法与avg相同）
-            avg1 = Meter1.select().avg(Meter1.cur,Meter1.curDouble.alias('aa')) #可以同时获取多列，并且可以使用别名
-            print(avg1.get(Meter1.cur.avg()),avg1.aa) #打印统计结果
-            #twa 必须配合where函数，且必须选择时间段
-            twa1 = Meter1.select().where(Meter1.ts > datetime.datetime(2020, 11, 19, 15, 9, 12, 946118),Meter1.ts < datetime.datetime.now()).twa(Meter1.cur,Meter1.curDouble.alias('aa'))
-            print(twa1.get(Meter1.cur.twa()),avg1.aa) #打印统计结果
-        
-            #diff
-            diffs = Meter1.select().diff(Meter1.curInt.alias('aa')) #diff目前只可以聚合一个属性。
-            for diff1 in diffs:
-                print(diff1.aa,diff1.ts) # 时间点数据同时返回
-        
-            #top(bottom函数使用方式相同)
-            tops = Meter1.select().top(Meter1.cur,3,alias='aa') # top函数需要提供要统计的属性，行数，以及别名
-            for top1 in tops:
-                print(top1.aa,top1.ts) # 时间点数据同时返回
-            tops = Meter1.select().top(Meter1.cur,3) # 可以不指定别名
-            for top1 in tops:
-                print(top1.get(Meter1.cur.top(3))) #不指定别名，需用使用get方法获取属性
-        
-            #percentile (apercentile函数使用方式相同) 
-            percentile1 = Meter1.select().percentile((Meter1.cur,1,'aa'),(Meter1.curDouble,2)) #每个属性参数为一个元组（数组），分别定义要统计的属性，P值（P值取值范围0≤P≤100），可选别名。
-            print(percentile1.aa)
-            print(percentile1.get(Meter1.curDouble.percentile(2)))#不指定别名，需用使用get方法获取属性
-        
-            #leastsquares
-            leastsquares1 = Meter1.select().leastsquares((Meter1.cur,1,1,'aa'),(Meter1.curDouble,2,2)) #每个属性参数为一个元组（数组），分别定义要统计的属性，start_val(自变量初始值)，step_val(自变量的步长值)，可选别名。
-            print(leastsquares1.aa) # 结果： {slop:-0.001595, intercept:0.212111}
-            print(leastsquares1.get(Meter1.curDouble.leastsquares(2,2))) #不指定别名，需用使用get方法获取属性
-        
-        group_by分组查询：
-        
-        .. code-block:: python
-        
-            # 可以在链式调用中加入group_by函数指定要分组的字段。然后在select函数中指定要分组统计的聚合函数（支持的聚合函数有：count、avg、sum 、stddev、leastsquares、percentile、min、max、first、last）
-            groups= Meter1.select(Meter1.desc,Meter1.curInt.avg().alias('intavg'),Meter1.cur.count().alias('curcount')).group_by(Meter1.desc).all()
-            for group in groups:
-                print(group.desc)
-                if group.desc == 'g1':
-                    # assert group.get(Meter1.curInt.count()) == 10
-                    assert group.intavg == 5.5
-                    assert group.curcount == 10
-                if group.desc == 'g2':
-                    assert group.intavg == 10.5
-                    assert group.curcount == 20
-        
-        时间维度聚合interval:
-        
-        .. code-block:: python
-        
-            # 可以使用interval函数调用TDengine时间纬度聚合功能,使用方法如下 时间间隔与offset参数参考TDengine文档（s:秒，m:分钟，h:小时）。fill参数可选字符串(NONE | PREV | NULL | LINEAR)或者任意数值,例如：fill=1.2将会以固定值填充。
-            results= Meter1.select(Meter1.cur.avg().alias('aa'),Meter1.cur.first().alias('bb')).where(Meter1.ts > (datetime.datetime.now()-datetime.timedelta(days=1))).interval('10s',fill='PREV',offset='1m').all()
-            for result in results:
-                print(result.aa,result.bb)
-        
-        join查询：
-        
-        目前并支持多表join查询，需要多表查询的情况请使用raw_sql函数，执行原始sql语句。以后的版本会补充此功能。
-        
-        
-        超级表定义：
-        
-        .. code-block:: python
-        
-            # 超级表模型类继承自SuperModel类
-            class Meters(SuperModel):
-                cur = FloatField(db_column='c1')
-                curInt = IntegerField(db_column='c2')
-                curDouble = DoubleField(db_column='c3')
-                desc = BinaryField(db_column='des')
-                class Meta:
-                    database = db
-                    db_table = 'meters'
-                    # Meta类中定义的Field，为超级表的标签
-                    location = BinaryField(max_length=30)
-                    groupid = IntegerField(db_column='gid')
-        
-        超级表的建表、删表、检查表是否存在：
-        
-        .. code-block:: python
-        
-            Meters.create_table(safe=True) #建表 safe：如果表存在，则跳过建表指令。命令运行成功放回True,失败raise错误
-            # db.create_table(Meters,safe=True) #通过数据库对象建表，功能同上
-            Meters.drop_table(safe=True) #删表 safe：如果表不存在，则跳过删表指令。命令运行成功放回True,失败raise错误
-            # db.drop_table(Meters,safe=True) #通过数据库对象删表，功能同上
-            Meters.supertable_exists() #查看表是否存在，存在返回True,不存在返回：False
-        
-        超级表动态建表：
-        
-        超级表除了使用定义模型类的方式建表外，也提供了动态定义字段建表的功能。
-        
-        .. code-block:: python
-        
-            #可以使用SuperModel类的类方法dynamic_create_table方法动态建表，第一个参数为表名，然后需要指定数据库，与是否安全建表
-            # 需要额外提供tags参数，参数值为一个字典(使用方法如下例)，设置超级表所有的标签。
-            # 关键词参数可以任意多个，指定表中的字段。
-            Meter_dynamic= SuperModel.dynamic_create_table('meterSD',database=db,safe=True,tags={'gid':IntegerField(db_column='tag1')},test1 = FloatField(db_column='t1'),test2 = IntegerField(db_column='t2'))
-            # 函数返回的对象为SuperModel类对象。使用方法与静态继承的模型类相同。
-            Meter_dynamic.supertable_exists()
-            Meter_dynamic.drop_table()
-        
-        从表名建立对应的supermodel类：
-        
-        数据库中已有的数据库超级表，可以通过已知的表名建立对应的supermodel类。
-        
-        .. code-block:: python
-        
-            sTable = SuperModel.supermodel_from_table('rule_10',db) # rule_10为数据表的表名
-            res = sTable.select().one() # 从表名新建的类和静态建立的类，使用方法完全一致
-        
-        从超级表建立子表：
-        
-        .. code-block:: python
-        
-            SonTable_d3 = Meters.create_son_table('d3',location='beijing',groupid=3) #生成字表模型类的同时，自动在数据库中建表。
-        
-            SonTable_d3.table_exists() # SonTable_d3的使用方法和继承自Modle类的模型类一样。可以进行插入与查询操作
-            # m = SonTable_d3(cur = 65.8,curInt=10,curDouble=1.1,desc='g1',ts = datetime.datetime.now())
-            # m.save()
-        
-        新增标签：
-        
-        .. code-block:: python
-        
-            # 使用add_tags方法，可以给超级表新建多个标签。每个参数可以是一个Field对象（必须指定db_column属性）
-            Meters.add_tags(IntegerField(db_column='add_tag_1'),IntegerField(db_column='add_tag_4'),BinaryField(max_length=30,db_column='add_tag_5'))
-        
-        删除标签：
-        
-        .. code-block:: python
-        
-            # 使用drop_tag方法可以删除超级表的标签，参数名为标签名，一次只能删除一个标签
-            Meters.drop_tag('add_tag_2')
-        
-        修改标签名：
-        
-        .. code-block:: python
-        
-            # 使用change_tag_name方法可以修改超级表的标签名，参数名为要修改的标签名，和新的标签名。（注意：此方法只修改对应超级表的标签名，并不修改类的属性名）
-            Meters.change_tag_name('add_tag_1','add_tag_2')
-        
-        
-        修改子表标签值：
-        
-        .. code-block:: python
-        
-            TableT = Meters.create_son_table('d3_insert',location='beijing',gid=3)
-            # 子表可以通过change_tag_value方法修改自己的标签值。
-            TableT.change_tag_value(location='tianjin',gid = 6)
-        
-        
-        
-        关于debug信息打印：
-        
-        如需查看crown调用tdengine引擎时执行的sql语句和返回的原始数据。只需要配置crown模块的logger记录器的日志输出级别为debug即可。
-        
-        .. code-block:: python
-        
-            import logging
-            from crown import logger
-        
-            logger.setLevel(logging.DEBUG) #配置logger对象，即可输出执行debug信息
-        
 Keywords: orm,taos,TDengine,TSDB,Time Series Database,connector,python
-Platform: UNKNOWN
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+crown
+======
+
+crown 是一个轻量级的针对时序数据（TSDB）TDengine的ORM库。 
+
+* 需要python 3.0版本以上
+* 0.1.7版本在tdengine 2版本测试通过
+* 0.3.0版本在tdengine 3版本测试通过
+* 解决mac操作系统下没有原生python连接器的问题
+* 极大的降低了python程序员使用TDengine技术门槛
+* 可以方便的将数据转换到numpy与pandas
+* 目前使用TDengine的restful接口连接数据库，以后将提供原生接口引擎可供选择（目前原生接口无法在mac系统上使用）
+
+安装
+----------------------
+
+大多数情况下，可以通过pip,轻松安装最新版本：
+
+.. code-block:: console
+
+    pip install crown
+
+
+还可以通过git安装，项目地址： https://github.com/machine-w/crown
+
+使用方法:
+
+.. code-block:: console
+
+    git clone https://github.com/machine-w/crown.git
+    cd crowm
+    python setup.py install
+
+
+使用文档
+------------------------
+
+建立数据库与删除数据库:
+
+.. code-block:: python
+
+    from crown import *
+
+    DATABASENAME = 'taos_test'
+    HOST = 'localhost'
+    PORT = 6041
+    # 默认端口 6041，默认用户名：root,默认密码：taosdata
+    db = TdEngineDatabase(DATABASENAME,host=HOST) #新建数据库对象
+    # db.connect()  # 尝试连接数据库，如果库不存在，则自动建库。
+    # print(db.databases) #连接数据库db对象后会自动获取全部数据库信息，以字典的形式保存在属性databases中。
+    # 如不使用默认值，可以如下传入参数
+    # db = TdEngineDatabase(DATABASENAME,host=HOST,port=PORT,user='yourusername',passwd='yourpassword')
+    db.create_database(safe=True)  #建库指令。 （safe：如果库存在，则跳过建库指令。）
+    # db.create_database(safe=True,keep= 100,comp=0,replica=1,quorum=2,blocks=115) #可选字段：建库时配置数据库参数，具体字段含义请参考tdengine文档。
+    db.drop_database(safe=True) #删库指令 （safe：如果库不存在，则跳过删库指令。）
+
+修改数据库参数:
+
+.. code-block:: python
+
+    db.alter_database(keep= 120,comp=1,replica=1,quorum=1,blocks=156) #同建库可选字段。
+
+执行sql语句:
+
+.. code-block:: python
+
+    #可以通过数据库对象直接执行sql语句，语句规则与TDengine restful接口要求一致。
+    res = db.raw_sql('select c1,c2 from taos_test.member1')
+    print(res,res.head,res.rowcount) #返回的对象为二维数据。res.head属性为数组对象，保存每一行数据的代表的列名。res.rowcount属性保存返回行数。
+    # res: [[1.2,2.2],[1.3,2.1],[1.5,2.0],[1.6,2.1]]
+    # res.head: ['c1','c2']
+    # res.rowcount: 4
+
+打印执行的sql语句:
+
+.. code-block:: python
+
+    Meter1.select().one()
+    print(db.curSql) #可以通过db对象的curSql属性获取当前执行的原始sql语句
+
+模型定义:
+
+.. code-block:: python
+
+    from crown import *
+
+    DATABASENAME = 'taos_test'
+    HOST = 'localhost'
+    db = TdEngineDatabase(DATABASENAME,host=HOST) #新建数据库对象
+    db.connect()  #尝试连接数据库，如果库不存在，则自动建库。
+    # print(db.databases) #连接数据库db对象后会自动获取全部数据库信息，以字典的形式保存在属性databases中。
+
+    # 表模型类继承自Model类，每个模型类对应数据库中的一张表，模型类中定义的每个Field，对应表中的一列
+    class Meter1(Model):
+        cur = FloatField(db_column='c1')
+        curInt = IntegerField(db_column='c2')
+        curDouble = DoubleField(db_column='c3')
+        desc = BinaryField(db_column='des')
+
+        class Meta: #Meta子类中定义模型类的配置信息
+            database = db #指定表所使用的数据库
+            db_table = 'meter1' #指定表名
+
+    # 可选择的全部Field类型如下，类型与Tdengine支持的数据类型一一对应
+    class AllField(Model):
+        name_float = FloatField(column_name='nf1') #可选项：指定列名
+        name_double = DoubleField()
+        name_bigint = BigIntegerField()
+        name_int = IntegerField()
+        name_smallint = SmallIntegerField()
+        name_tinyint = TinyIntegerField()
+        name_nchar = NCharField(max_length=59,db_column='n1')
+        name_binary = BinaryField(max_length=3)
+        name_bool = BooleanField()
+        dd = PrimaryKeyField() # 如果定义了主键列，则使用主键列作为主键，如果没有定义，则默认“ts”为主键。
+        birthday = DateTimeField()
+        class Meta:
+            database = db
+            db_table = 'all_field'
+
+主键定义：
+
+.. code-block:: python
+
+    #定义主键方式1 
+    #不定义主键，系统默认主键：“ts”
+    class TestPri(Model):
+        cur = FloatField(db_column='c1')
+        class Meta:
+            database = db
+    res = TestPri.describe_table() #获取表结构信息
+    print(res[0][0]) # 结果: “ts”
+
+    #定义主键方式2
+    class TestPri(Model):
+        cur = FloatField(db_column='c1')
+        timeline = PrimaryKeyField() #定义主键列，主键名设置为列名
+        class Meta:
+            database = db
+    res = TestPri.describe_table()
+    print(res[0][0]) # 结果: “timeline”
+
+     #定义主键方式3
+    class TestPri(Model):
+        cur = FloatField(db_column='c1')
+        class Meta:
+            database = db
+            primary_key = 'timeline' # Meta中定主键名称
+    res = TestPri.describe_table()
+    print(res[0][0]) # 结果: “timeline”
+    
+
+
+建表、删表、检查表是否存在：
+
+.. code-block:: python
+
+    Meter1.create_table(safe=True) #建表 safe：如果表存在，则跳过建表指令。命令运行成功放回True,失败raise错误
+    # db.create_table(Meter1,safe=True) #通过数据库对象建表，功能同上
+    Meter1.drop_table(safe=True) #删表 safe：如果表不存在，则跳过删表指令。命令运行成功放回True,失败raise错误
+    # db.drop_table(Meter1,safe=True) #通过数据库对象删表，功能同上
+    Meter1.table_exists() #查看表是否存在，存在返回True,不存在返回：False
+
+动态建表：
+
+除了使用定义模型类的方式建表外，还提供了动态定义字段建表的功能。
+
+.. code-block:: python
+
+    #可以使用Model类的类方法dynamic_create_table方法动态建表，第一个参数为表名，然后需要指定数据库，与是否安全建表。
+    # 关键词参数可以任意多个，指定表中的字段。
+    Meter_dynamic= Model.dynamic_create_table('meterD',database=db,safe=True,test1 = FloatField(db_column='t1'),test2 = IntegerField(db_column='t2'))
+    # 函数返回的对象为Model类对象。使用方法与静态继承的模型类相同。
+    Meter_dynamic.table_exists()
+    Meter_dynamic.drop_table()
+
+从表名建立对应的model类：
+
+数据库中已有的数据库表，可以通过已知的表名建立对应的model类。
+
+.. code-block:: python
+
+    nodeTable = Model.model_from_table('node_10',db) # node_10为数据表的表名
+    res = nodeTable.select().one() # 从表名新建的类和静态建立的类，使用方法完全一致
+    
+    
+动态建立的或从数据库分析得到的model对象，可以直接使用列名作为属性名进行查询操作。
+
+.. code-block:: python
+
+
+    res = nodeTable.select(nodeTable.c1)where(nodeTable.c1 > 1).all() # 直接使用列名
+    res = nodeTable.select(nodeTable.c1)where(FloatField(db_column='c1') > 1).all() # 也可以使用field对象作为字段检索条件（多使用于列名为动态值的时候）
+    # 直接使用列名,查看结果
+    for item in res:
+        print(item.c1)
+
+插入数据：
+
+.. code-block:: python
+
+    #方法一
+    for i in range(1,101):
+        #使用模型类实例化的每个对象对应数据表中的每一行，可以通过传入属性参数的方式给每一列赋值
+        m = Meter1(cur = 1/i,curInt=i,curDouble=1/i+10,desc='g1',ts= datetime.datetime.now() - datetime.timedelta(seconds=(102-i)))
+        #使用对象的save方法将数据存入数据库
+        m.save()
+    print(Meter1.select().count()) # 结果：100
+    #方法二
+    for i in range(1,11):
+        #也可以直接使用模型类的insert方法插入数据。
+        Meter1.insert(cur = 1/i,curInt=i,curDouble=1/i+10,desc='g1',ts= datetime.datetime.now() - datetime.timedelta(seconds=(12-i)))
+    print(Meter1.select().count()) # 结果：100
+    #如果不传入时间属性，则会以当前时刻为默认值传入
+    Meter1.insert(cur = 1/i,curInt=i,curDouble=1/i+10,desc='g1')
+    m = Meter1(cur = 1/i,curInt=i,curDouble=1/i+10,desc='g1')
+    m.save()
+
+查询单条数据：
+
+.. code-block:: python
+
+    #获取一条数据
+    #使用select()类方法获取查询字段（参数留空表示取全部字段），然后可以链式使用one方法获取第一条数据
+    res = Meter1.select().one()
+    print(res.desc,res.curDouble,res.curInt,res.cur,res.ts)
+
+    #select函数中可以选择要读取的字段
+    res = Meter1.select(Meter1.cur,Meter1.desc).one()
+    print(res.desc,res.curDouble,res.curInt,res.cur,res.ts)
+
+    #select函数中可以使用Model的类方法f()和fc()获取字符串形式的属性名与列名对应Field对象
+    res = Meter1.select(Meter1.f('cur'),Meter1.fc('c3'),Meter1.desc).one()
+    print(res.desc,res.curDouble,res.curInt,res.fc('c3'),res.f('cur'),res.ts)
+
+查询全部数据：
+
+.. code-block:: python
+
+    #获取一条数据
+    #使用select()类方法获取查询字段（参数留空表示取全部字段），然后可以链式使用all方法获取全部数据
+    res_all = Meter1.select().all()
+    for res in res_all:
+        print(res.desc,res.curDouble,res.curInt,res.cur,res.ts)
+
+    #select函数中可以选择要读取的字段
+    res_all = Meter1.select(Meter1.cur,Meter1.desc).all()
+    for res in res_all:
+        print(res.desc,res.curDouble,res.curInt,res.cur,res.ts)
+
+虽然TDengine提供了很多聚合和统计函数，但是把时序数据导入numpy或pandas等数据分析组件中进行处理的情况也是很常见的操作。
+下面介绍如何通过crown把结果数据导入numpy和pandas
+
+读取数据到numpy：
+
+.. code-block:: python
+
+    #通过all_raw函数可以获取二维数组格式的数据查询结果。结果每列代表的标题保存在结果对象的head属性中。
+    raw_results = Meter1.select(Meter1.cur,Meter1.curInt,Meter1.curDouble).all_raw()
+    #可以很方便的将结果转换为numpy数组对象
+    np_data = np.array(raw_results)
+    print(np_data)
+    print(raw_results.head)
+
+读取数据到pandas：
+
+.. code-block:: python
+
+    raw_results = Meter1.select().all_raw()
+    #使用以下方法，可以轻松的将数据导入pandas,并且使用时间点作为index,使用返回的数据标题作为列名。
+    pd_data = pd.DataFrame(raw_results,columns=raw_results.head).set_index('ts')
+    print(pd_data)
+
+选择列四则运算：
+
+.. code-block:: python
+
+    #使用select()类方法获取查询字段时，可以返回某列或多列间的值加、减、乘、除、取余计算结果（+ - * / %）
+    res_all = Meter1.select((Meter1.curDouble+Meter1.cur),Meter1.ts).all()
+    for res in res_all:
+        print(res.get(Meter1.curDouble+Meter1.cur),res.ts) #返回的结果对象可以用get方法获取原始计算式结果
+
+    #字段别名
+    res_all = Meter1.select(((Meter1.curDouble+Meter1.cur)*Meter1.curDouble).alias('new_name'),Meter1.ts).all() #给运算式起别名（不仅运算式，其他放在select函数中的任何属性都可以使用别名）
+    for res in res_all:
+        print(res.new_name,res.ts) #使用别名获取运算结果
+
+where查询条件：
+
+.. code-block:: python
+
+    #可以在select函数后链式调用where函数进行条件限
+    one_time =datetime.datetime.now() - datetime.timedelta(hours=10)
+    ress = Meter1.select().where(Meter1.ts > one_time).all()
+    #限定条件可以使用 > < == >= <= != and or ! 等。字符类型的字段可以使用 % 作为模糊查询（相当于like）
+    # 逻辑操作符号 |: 或 &：与 ~：非。（注意：做逻辑操作符号的表达式需要用括号括起来）
+    ress = Meter1.select().where((Meter1.cur > 0) | (Meter1.desc % 'g%')).all()
+    #where函数可以接收任意多参数，每个参数为一个限定条件，参数条件之间为"与"的关系。
+    ress = Meter1.select().where(Meter1.cur > 0, Meter1.ts > one_time, Meter1.desc % '%1').all()
+
+分页与limit：
+
+.. code-block:: python
+
+    #可以在select函数后链式调用paginate函数进行分页操作，以下例子为取第6页 每页5条数据。
+    ress_1 = Meter1.select().paginate(6,page_size=5).all()
+    ress_2 = Meter1.select().paginate(6).all() #默认page_size为20
+    #可以在select函数后链式调用limit函数和offset函数条数限制和定位操作。
+    ress_3 = Meter1.select().limit(2).offset(5).all()
+    ress_4 = Meter1.select().limit(2).all()
+
+排序（目前tdengine只支持主键排序）：
+
+.. code-block:: python
+
+    #可以在select函数后链式调用desc或者asc函数进行时间轴的正序或者倒序查询
+    res = Meter1.select().desc().one()
+    #定义模型类的时候定义默认排序方法
+    class Meter1(Model):
+        cur = FloatField(db_column='c1')
+        curInt = IntegerField(db_column='c2')
+        curDouble = DoubleField(db_column='c3')
+        desc = BinaryField(db_column='des')
+        dd = PrimaryKeyField().desc() #可以在定义主键的时候调用field的desc或asc方法定义默认排序
+        class Meta:
+            # order_by= ['-dd'] #也可以在元数据类中定义‘-dd’代表倒序‘dd’ 代表正序
+            database = db
+
+去重 ：
+
+.. code-block:: python
+
+    #可以在select函数后链式调用distinct函数对返回的数据列进行去重复操作
+    res = Meter1.select().distinct().all()
+
+聚合函数：
+
+.. code-block:: python
+
+    #count
+    count = Meter1.select().count() #统计行数
+    print(count) # 结果： 100
+    count = Meter1.select().count(Meter1.desc) #统计指定列非空行数
+    print(count) # 结果： 90
+    #avg（sum,stddev,min,max,first,last,last_row,spread使用方法与avg相同）
+    avg1 = Meter1.select().avg(Meter1.cur,Meter1.curDouble.alias('aa')) #可以同时获取多列，并且可以使用别名
+    print(avg1.get(Meter1.cur.avg()),avg1.aa) #打印统计结果
+    #twa 必须配合where函数，且必须选择时间段
+    twa1 = Meter1.select().where(Meter1.ts > datetime.datetime(2020, 11, 19, 15, 9, 12, 946118),Meter1.ts < datetime.datetime.now()).twa(Meter1.cur,Meter1.curDouble.alias('aa'))
+    print(twa1.get(Meter1.cur.twa()),avg1.aa) #打印统计结果
+
+    #diff
+    diffs = Meter1.select().diff(Meter1.curInt.alias('aa')) #diff目前只可以聚合一个属性。
+    for diff1 in diffs:
+        print(diff1.aa,diff1.ts) # 时间点数据同时返回
+
+    #top(bottom函数使用方式相同)
+    tops = Meter1.select().top(Meter1.cur,3,alias='aa') # top函数需要提供要统计的属性，行数，以及别名
+    for top1 in tops:
+        print(top1.aa,top1.ts) # 时间点数据同时返回
+    tops = Meter1.select().top(Meter1.cur,3) # 可以不指定别名
+    for top1 in tops:
+        print(top1.get(Meter1.cur.top(3))) #不指定别名，需用使用get方法获取属性
+
+    #percentile (apercentile函数使用方式相同) 
+    percentile1 = Meter1.select().percentile((Meter1.cur,1,'aa'),(Meter1.curDouble,2)) #每个属性参数为一个元组（数组），分别定义要统计的属性，P值（P值取值范围0≤P≤100），可选别名。
+    print(percentile1.aa)
+    print(percentile1.get(Meter1.curDouble.percentile(2)))#不指定别名，需用使用get方法获取属性
+
+    #leastsquares
+    leastsquares1 = Meter1.select().leastsquares((Meter1.cur,1,1,'aa'),(Meter1.curDouble,2,2)) #每个属性参数为一个元组（数组），分别定义要统计的属性，start_val(自变量初始值)，step_val(自变量的步长值)，可选别名。
+    print(leastsquares1.aa) # 结果： {slop:-0.001595, intercept:0.212111}
+    print(leastsquares1.get(Meter1.curDouble.leastsquares(2,2))) #不指定别名，需用使用get方法获取属性
+
+group_by分组查询：
+
+.. code-block:: python
+
+    # 可以在链式调用中加入group_by函数指定要分组的字段。然后在select函数中指定要分组统计的聚合函数（支持的聚合函数有：count、avg、sum 、stddev、leastsquares、percentile、min、max、first、last）
+    groups= Meter1.select(Meter1.desc,Meter1.curInt.avg().alias('intavg'),Meter1.cur.count().alias('curcount')).group_by(Meter1.desc).all()
+    for group in groups:
+        print(group.desc)
+        if group.desc == 'g1':
+            # assert group.get(Meter1.curInt.count()) == 10
+            assert group.intavg == 5.5
+            assert group.curcount == 10
+        if group.desc == 'g2':
+            assert group.intavg == 10.5
+            assert group.curcount == 20
+
+时间维度聚合interval:
+
+.. code-block:: python
+
+    # 可以使用interval函数调用TDengine时间纬度聚合功能,使用方法如下 时间间隔与offset参数参考TDengine文档（s:秒，m:分钟，h:小时）。fill参数可选字符串(NONE | PREV | NULL | LINEAR)或者任意数值,例如：fill=1.2将会以固定值填充。
+    results= Meter1.select(Meter1.cur.avg().alias('aa'),Meter1.cur.first().alias('bb')).where(Meter1.ts > (datetime.datetime.now()-datetime.timedelta(days=1))).interval('10s',fill='PREV',offset='1m').all()
+    for result in results:
+        print(result.aa,result.bb)
+
+join查询：
+
+目前并支持多表join查询，需要多表查询的情况请使用raw_sql函数，执行原始sql语句。以后的版本会补充此功能。
+
+
+超级表定义：
+
+.. code-block:: python
+
+    # 超级表模型类继承自SuperModel类
+    class Meters(SuperModel):
+        cur = FloatField(db_column='c1')
+        curInt = IntegerField(db_column='c2')
+        curDouble = DoubleField(db_column='c3')
+        desc = BinaryField(db_column='des')
+        class Meta:
+            database = db
+            db_table = 'meters'
+            # Meta类中定义的Field，为超级表的标签
+            location = BinaryField(max_length=30)
+            groupid = IntegerField(db_column='gid')
+
+超级表的建表、删表、检查表是否存在：
+
+.. code-block:: python
+
+    Meters.create_table(safe=True) #建表 safe：如果表存在，则跳过建表指令。命令运行成功放回True,失败raise错误
+    # db.create_table(Meters,safe=True) #通过数据库对象建表，功能同上
+    Meters.drop_table(safe=True) #删表 safe：如果表不存在，则跳过删表指令。命令运行成功放回True,失败raise错误
+    # db.drop_table(Meters,safe=True) #通过数据库对象删表，功能同上
+    Meters.supertable_exists() #查看表是否存在，存在返回True,不存在返回：False
+
+超级表动态建表：
+
+超级表除了使用定义模型类的方式建表外，也提供了动态定义字段建表的功能。
+
+.. code-block:: python
+
+    #可以使用SuperModel类的类方法dynamic_create_table方法动态建表，第一个参数为表名，然后需要指定数据库，与是否安全建表
+    # 需要额外提供tags参数，参数值为一个字典(使用方法如下例)，设置超级表所有的标签。
+    # 关键词参数可以任意多个，指定表中的字段。
+    Meter_dynamic= SuperModel.dynamic_create_table('meterSD',database=db,safe=True,tags={'gid':IntegerField(db_column='tag1')},test1 = FloatField(db_column='t1'),test2 = IntegerField(db_column='t2'))
+    # 函数返回的对象为SuperModel类对象。使用方法与静态继承的模型类相同。
+    Meter_dynamic.supertable_exists()
+    Meter_dynamic.drop_table()
+
+从表名建立对应的supermodel类：
+
+数据库中已有的数据库超级表，可以通过已知的表名建立对应的supermodel类。
+
+.. code-block:: python
+
+    sTable = SuperModel.supermodel_from_table('rule_10',db) # rule_10为数据表的表名
+    res = sTable.select().one() # 从表名新建的类和静态建立的类，使用方法完全一致
+
+从超级表建立子表：
+
+.. code-block:: python
+
+    SonTable_d3 = Meters.create_son_table('d3',location='beijing',groupid=3) #生成字表模型类的同时，自动在数据库中建表。
+
+    SonTable_d3.table_exists() # SonTable_d3的使用方法和继承自Modle类的模型类一样。可以进行插入与查询操作
+    # m = SonTable_d3(cur = 65.8,curInt=10,curDouble=1.1,desc='g1',ts = datetime.datetime.now())
+    # m.save()
+
+新增标签：
+
+.. code-block:: python
+
+    # 使用add_tags方法，可以给超级表新建多个标签。每个参数可以是一个Field对象（必须指定db_column属性）
+    Meters.add_tags(IntegerField(db_column='add_tag_1'),IntegerField(db_column='add_tag_4'),BinaryField(max_length=30,db_column='add_tag_5'))
+
+删除标签：
+
+.. code-block:: python
+
+    # 使用drop_tag方法可以删除超级表的标签，参数名为标签名，一次只能删除一个标签
+    Meters.drop_tag('add_tag_2')
+
+修改标签名：
+
+.. code-block:: python
+
+    # 使用change_tag_name方法可以修改超级表的标签名，参数名为要修改的标签名，和新的标签名。（注意：此方法只修改对应超级表的标签名，并不修改类的属性名）
+    Meters.change_tag_name('add_tag_1','add_tag_2')
+
+
+修改子表标签值：
+
+.. code-block:: python
+
+    TableT = Meters.create_son_table('d3_insert',location='beijing',gid=3)
+    # 子表可以通过change_tag_value方法修改自己的标签值。
+    TableT.change_tag_value(location='tianjin',gid = 6)
+
+
+
+关于debug信息打印：
+
+如需查看crown调用tdengine引擎时执行的sql语句和返回的原始数据。只需要配置crown模块的logger记录器的日志输出级别为debug即可。
+
+.. code-block:: python
+
+    import logging
+    from crown import logger
+
+    logger.setLevel(logging.DEBUG) #配置logger对象，即可输出执行debug信息
```

### Comparing `crown-0.1.7/README.rst` & `crown-0.3.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 crown
 ======
 
 crown 是一个轻量级的针对时序数据（TSDB）TDengine的ORM库。 
 
 * 需要python 3.0版本以上
-* 在tdengine 2.0.8版本测试通过
+* 0.1.7版本在tdengine 2版本测试通过
+* 0.3.0版本在tdengine 3版本测试通过
 * 解决mac操作系统下没有原生python连接器的问题
 * 极大的降低了python程序员使用TDengine技术门槛
 * 可以方便的将数据转换到numpy与pandas
 * 目前使用TDengine的restful接口连接数据库，以后将提供原生接口引擎可供选择（目前原生接口无法在mac系统上使用）
 
 安装
 ----------------------
```

### Comparing `crown-0.1.7/crown/common.py` & `crown-0.3.0/crown/common.py`

 * *Files identical despite different names*

### Comparing `crown-0.1.7/crown/crown.py` & `crown-0.3.0/crown/crown.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,14 +183,16 @@
                         val = SmallIntegerField(column_name=f[0])
                     elif f[1] == 'TINYINT':
                         val = TinyIntegerField(column_name=f[0])
                     elif f[1] == 'NCHAR':
                         val = NCharField(column_name=f[0],max_length=f[2])
                     elif f[1] == 'BINARY':
                         val = BinaryField(column_name=f[0],max_length=f[2])
+                    elif f[1] == 'VARCHAR':
+                        val = VarCharField(column_name=f[0],max_length=f[2])
                     elif f[1] == 'BOOL':
                         val = BooleanField(column_name=f[0])
                     else:
                         raise Exception('have unknow field')
                     fields[f[0]] = val
             resModel = type(table_name, (cls,), fields)
             return resModel
@@ -313,14 +315,16 @@
                     val = SmallIntegerField(column_name=f[0])
                 elif f[1] == 'TINYINT':
                     val = TinyIntegerField(column_name=f[0])
                 elif f[1] == 'NCHAR':
                     val = NCharField(column_name=f[0],max_length=f[2])
                 elif f[1] == 'BINARY':
                     val = BinaryField(column_name=f[0],max_length=f[2])
+                elif f[1] == 'VARCHAR':
+                    val = VarCharField(column_name=f[0],max_length=f[2])
                 elif f[1] == 'BOOL':
                     val = BooleanField(column_name=f[0])
                 else:
                     raise Exception('have unknow field')
                 if f[3] == 'TAG':
                     tags[f[0]] = val
                 else:
```

### Comparing `crown-0.1.7/crown/database.py` & `crown-0.3.0/crown/database.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import threading
 from .common import *
 from .query import *
-from .eng_taosrestful import taos_resetful
 class Database(object):
     commit_select = False
     compiler_class = QueryCompiler
     empty_limit = False
     field_overrides = {}
     for_update = False
     interpolation = '{}'
@@ -186,10 +185,15 @@
         return self.execute_sql(qc.drop_tag(model_class,name))
     def change_tag_name(self, model_class,name,newname):
         qc = self.get_compiler()
         return self.execute_sql(qc.change_tag_name(model_class,name,newname))
     def raw_sql(self, sql, *params):
         return self.execute_sql(sql.replace("?", "{}"),params)
 class TdEngineDatabase(Database):
-    def _connect(self, database, **kwargs):
-        return taos_resetful.connect(database=database, **kwargs)
+    def _connect(self, database, version=3,**kwargs):
+        if version ==2:
+            from .eng_taosrestful import taos_resetful
+            return taos_resetful.connect(database=database, **kwargs)
+        elif version ==3:
+            from .eng_taosrestful3 import taos_resetful
+            return taos_resetful.connect(database=database, **kwargs)
 default_database = TdEngineDatabase('demo',host='localhost')
```

### Comparing `crown-0.1.7/crown/eng_taosrestful.py` & `crown-0.3.0/crown/eng_taosrestful.py`

 * *Files identical despite different names*

### Comparing `crown-0.1.7/crown/field.py` & `crown-0.3.0/crown/field.py`

 * *Files 4% similar despite different names*

```diff
@@ -248,23 +248,26 @@
     post_process = post_process or (lambda x: x)
     for fmt in formats:
         try:
             return post_process(datetime.datetime.strptime(value, fmt))
         except ValueError:
             pass
     return value
+class VarCharField(BinaryField):
+    db_field = 'varchar'
 class DateTimeField(Field):
     db_field = 'datetime'
 
     def field_attributes(self):
         return {
             'formats': [
-                '%Y-%m-%d %H:%M:%S.%f',
-                '%Y-%m-%d %H:%M:%S',
-                '%Y-%m-%d',
+                '%Y-%m-%dT%H:%M:%S.%fZ'
+                # '%Y-%m-%d %H:%M:%S.%f',
+                # '%Y-%m-%d %H:%M:%S',
+                # '%Y-%m-%d',
             ]
         }
 
     def python_value(self, value):
         if value and isinstance(value, str):
             return format_date_time(value, self.attributes['formats'])
         return value
```

### Comparing `crown-0.1.7/crown/query.py` & `crown-0.3.0/crown/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
         'smallint': 'SMALLINT',
         'tinyint': 'TINYINT',
         'bigint': 'BIGINT',
         'float': 'FLOAT',
         'double': 'DOUBLE',
         'nchar': 'NCHAR',
         'binary': 'BINARY',
+        'varchar': 'VARCHAR',
         'datetime': 'TIMESTAMP',
         'bool': 'BOOL',
         'primary_key': 'TIMESTAMP',
     }
 
     op_map = {
         OP_EQ: '=',
@@ -45,15 +46,18 @@
                  op_overrides=None):
         self.quote_char = quote_char
         self.interpolation = interpolation
         self._field_map = dict_update(self.field_map, field_overrides or {})
         self._op_map = dict_update(self.op_map, op_overrides or {})
 
     def quote(self, s):
-        return ''.join((self.quote_char, s, self.quote_char))
+        # if TAOS_VERSION ==2:
+        #     return ''.join((self.quote_char, s, self.quote_char))
+        # elif TAOS_VERSION ==3:
+        return s
 
     def get_field(self, f):
         return self._field_map[f]
 
     def get_op(self, q):
         return self._op_map[q]
 
@@ -294,17 +298,17 @@
         parts.append(self.quote(model_class._meta.db_table))
         return ' '.join(parts)
     def change_table_tagvalue(self,model_class,name,value):
         parts = ['ALTER TABLE ']
         parts.append(model_class._meta.db_table) #TODO：restful api 对引号的表名支持不好
         # parts.append(self.quote(model_class._meta.db_table))
         if isinstance(value,str):
-            parts.append('SET TAG "%s" = "%s"' % (name,value))
+            parts.append('SET TAG %s = "%s"' % (name,value))
         else:
-            parts.append('SET TAG "%s" = %s' % (name,value))
+            parts.append('SET TAG %s = %s' % (name,value))
         return ' '.join(parts)
     def add_tag(self,model_class,value):
         parts = ['ALTER TABLE ']
         parts.append(model_class._meta.db_table) #TODO：restful api 对引号的表名支持不好
         # parts.append(self.quote(model_class._meta.db_table))
         if isinstance(value, Field) and not isinstance(value, DateTimeField) and value.db_column:
             parts.append('ADD TAG %s' % (self.field_sql(value)))
@@ -315,15 +319,15 @@
         # parts.append(self.quote(model_class._meta.db_table))
         parts.append('DROP TAG %s' % (name))
         return ' '.join(parts)
     def change_tag_name(self,model_class,name,newname):
         parts = ['ALTER TABLE ']
         parts.append(model_class._meta.db_table) #TODO：restful api 对引号的表名支持不好
         # parts.append(self.quote(model_class._meta.db_table))
-        parts.append('CHANGE TAG %s %s' % (name,newname))
+        parts.append('RENAME TAG %s %s' % (name,newname))
         return ' '.join(parts)
     def drop_table(self, model_class, fail_silently=False, cascade=False):
         parts = ['DROP TABLE']
         if fail_silently:
             parts.append('IF EXISTS')
         parts.append(self.quote(model_class._meta.db_table))
         return ' '.join(parts)
```

### Comparing `crown-0.1.7/crown.egg-info/PKG-INFO` & `crown-0.3.0/crown.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,518 +1,518 @@
 Metadata-Version: 2.1
 Name: crown
-Version: 0.1.7
+Version: 0.3.0
 Summary: crown is a simple and small ORM for Time Series Database (TSDB) tdengine(taos), making it easy to learn and intuitive to use.
 Home-page: https://github.com/machine-w/crown
 Author: machine-w
 Author-email: steve2008.ma@gmail.com
-License: UNKNOWN
-Description: crown
-        ======
-        
-        crown 是一个轻量级的针对时序数据（TSDB）TDengine的ORM库。 
-        
-        * 需要python 3.0版本以上
-        * 在tdengine 2.0.8版本测试通过
-        * 解决mac操作系统下没有原生python连接器的问题
-        * 极大的降低了python程序员使用TDengine技术门槛
-        * 可以方便的将数据转换到numpy与pandas
-        * 目前使用TDengine的restful接口连接数据库，以后将提供原生接口引擎可供选择（目前原生接口无法在mac系统上使用）
-        
-        安装
-        ----------------------
-        
-        大多数情况下，可以通过pip,轻松安装最新版本：
-        
-        .. code-block:: console
-        
-            pip install crown
-        
-        
-        还可以通过git安装，项目地址： https://github.com/machine-w/crown
-        
-        使用方法:
-        
-        .. code-block:: console
-        
-            git clone https://github.com/machine-w/crown.git
-            cd crowm
-            python setup.py install
-        
-        
-        使用文档
-        ------------------------
-        
-        建立数据库与删除数据库:
-        
-        .. code-block:: python
-        
-            from crown import *
-        
-            DATABASENAME = 'taos_test'
-            HOST = 'localhost'
-            PORT = 6041
-            # 默认端口 6041，默认用户名：root,默认密码：taosdata
-            db = TdEngineDatabase(DATABASENAME,host=HOST) #新建数据库对象
-            # db.connect()  # 尝试连接数据库，如果库不存在，则自动建库。
-            # print(db.databases) #连接数据库db对象后会自动获取全部数据库信息，以字典的形式保存在属性databases中。
-            # 如不使用默认值，可以如下传入参数
-            # db = TdEngineDatabase(DATABASENAME,host=HOST,port=PORT,user='yourusername',passwd='yourpassword')
-            db.create_database(safe=True)  #建库指令。 （safe：如果库存在，则跳过建库指令。）
-            # db.create_database(safe=True,keep= 100,comp=0,replica=1,quorum=2,blocks=115) #可选字段：建库时配置数据库参数，具体字段含义请参考tdengine文档。
-            db.drop_database(safe=True) #删库指令 （safe：如果库不存在，则跳过删库指令。）
-        
-        修改数据库参数:
-        
-        .. code-block:: python
-        
-            db.alter_database(keep= 120,comp=1,replica=1,quorum=1,blocks=156) #同建库可选字段。
-        
-        执行sql语句:
-        
-        .. code-block:: python
-        
-            #可以通过数据库对象直接执行sql语句，语句规则与TDengine restful接口要求一致。
-            res = db.raw_sql('select c1,c2 from taos_test.member1')
-            print(res,res.head,res.rowcount) #返回的对象为二维数据。res.head属性为数组对象，保存每一行数据的代表的列名。res.rowcount属性保存返回行数。
-            # res: [[1.2,2.2],[1.3,2.1],[1.5,2.0],[1.6,2.1]]
-            # res.head: ['c1','c2']
-            # res.rowcount: 4
-        
-        打印执行的sql语句:
-        
-        .. code-block:: python
-        
-            Meter1.select().one()
-            print(db.curSql) #可以通过db对象的curSql属性获取当前执行的原始sql语句
-        
-        模型定义:
-        
-        .. code-block:: python
-        
-            from crown import *
-        
-            DATABASENAME = 'taos_test'
-            HOST = 'localhost'
-            db = TdEngineDatabase(DATABASENAME,host=HOST) #新建数据库对象
-            db.connect()  #尝试连接数据库，如果库不存在，则自动建库。
-            # print(db.databases) #连接数据库db对象后会自动获取全部数据库信息，以字典的形式保存在属性databases中。
-        
-            # 表模型类继承自Model类，每个模型类对应数据库中的一张表，模型类中定义的每个Field，对应表中的一列
-            class Meter1(Model):
-                cur = FloatField(db_column='c1')
-                curInt = IntegerField(db_column='c2')
-                curDouble = DoubleField(db_column='c3')
-                desc = BinaryField(db_column='des')
-        
-                class Meta: #Meta子类中定义模型类的配置信息
-                    database = db #指定表所使用的数据库
-                    db_table = 'meter1' #指定表名
-        
-            # 可选择的全部Field类型如下，类型与Tdengine支持的数据类型一一对应
-            class AllField(Model):
-                name_float = FloatField(column_name='nf1') #可选项：指定列名
-                name_double = DoubleField()
-                name_bigint = BigIntegerField()
-                name_int = IntegerField()
-                name_smallint = SmallIntegerField()
-                name_tinyint = TinyIntegerField()
-                name_nchar = NCharField(max_length=59,db_column='n1')
-                name_binary = BinaryField(max_length=3)
-                name_bool = BooleanField()
-                dd = PrimaryKeyField() # 如果定义了主键列，则使用主键列作为主键，如果没有定义，则默认“ts”为主键。
-                birthday = DateTimeField()
-                class Meta:
-                    database = db
-                    db_table = 'all_field'
-        
-        主键定义：
-        
-        .. code-block:: python
-        
-            #定义主键方式1 
-            #不定义主键，系统默认主键：“ts”
-            class TestPri(Model):
-                cur = FloatField(db_column='c1')
-                class Meta:
-                    database = db
-            res = TestPri.describe_table() #获取表结构信息
-            print(res[0][0]) # 结果: “ts”
-        
-            #定义主键方式2
-            class TestPri(Model):
-                cur = FloatField(db_column='c1')
-                timeline = PrimaryKeyField() #定义主键列，主键名设置为列名
-                class Meta:
-                    database = db
-            res = TestPri.describe_table()
-            print(res[0][0]) # 结果: “timeline”
-        
-             #定义主键方式3
-            class TestPri(Model):
-                cur = FloatField(db_column='c1')
-                class Meta:
-                    database = db
-                    primary_key = 'timeline' # Meta中定主键名称
-            res = TestPri.describe_table()
-            print(res[0][0]) # 结果: “timeline”
-            
-        
-        
-        建表、删表、检查表是否存在：
-        
-        .. code-block:: python
-        
-            Meter1.create_table(safe=True) #建表 safe：如果表存在，则跳过建表指令。命令运行成功放回True,失败raise错误
-            # db.create_table(Meter1,safe=True) #通过数据库对象建表，功能同上
-            Meter1.drop_table(safe=True) #删表 safe：如果表不存在，则跳过删表指令。命令运行成功放回True,失败raise错误
-            # db.drop_table(Meter1,safe=True) #通过数据库对象删表，功能同上
-            Meter1.table_exists() #查看表是否存在，存在返回True,不存在返回：False
-        
-        动态建表：
-        
-        除了使用定义模型类的方式建表外，还提供了动态定义字段建表的功能。
-        
-        .. code-block:: python
-        
-            #可以使用Model类的类方法dynamic_create_table方法动态建表，第一个参数为表名，然后需要指定数据库，与是否安全建表。
-            # 关键词参数可以任意多个，指定表中的字段。
-            Meter_dynamic= Model.dynamic_create_table('meterD',database=db,safe=True,test1 = FloatField(db_column='t1'),test2 = IntegerField(db_column='t2'))
-            # 函数返回的对象为Model类对象。使用方法与静态继承的模型类相同。
-            Meter_dynamic.table_exists()
-            Meter_dynamic.drop_table()
-        
-        从表名建立对应的model类：
-        
-        数据库中已有的数据库表，可以通过已知的表名建立对应的model类。
-        
-        .. code-block:: python
-        
-            nodeTable = Model.model_from_table('node_10',db) # node_10为数据表的表名
-            res = nodeTable.select().one() # 从表名新建的类和静态建立的类，使用方法完全一致
-            
-            
-        动态建立的或从数据库分析得到的model对象，可以直接使用列名作为属性名进行查询操作。
-        
-        .. code-block:: python
-        
-        
-            res = nodeTable.select(nodeTable.c1)where(nodeTable.c1 > 1).all() # 直接使用列名
-            res = nodeTable.select(nodeTable.c1)where(FloatField(db_column='c1') > 1).all() # 也可以使用field对象作为字段检索条件（多使用于列名为动态值的时候）
-            # 直接使用列名,查看结果
-            for item in res:
-                print(item.c1)
-        
-        插入数据：
-        
-        .. code-block:: python
-        
-            #方法一
-            for i in range(1,101):
-                #使用模型类实例化的每个对象对应数据表中的每一行，可以通过传入属性参数的方式给每一列赋值
-                m = Meter1(cur = 1/i,curInt=i,curDouble=1/i+10,desc='g1',ts= datetime.datetime.now() - datetime.timedelta(seconds=(102-i)))
-                #使用对象的save方法将数据存入数据库
-                m.save()
-            print(Meter1.select().count()) # 结果：100
-            #方法二
-            for i in range(1,11):
-                #也可以直接使用模型类的insert方法插入数据。
-                Meter1.insert(cur = 1/i,curInt=i,curDouble=1/i+10,desc='g1',ts= datetime.datetime.now() - datetime.timedelta(seconds=(12-i)))
-            print(Meter1.select().count()) # 结果：100
-            #如果不传入时间属性，则会以当前时刻为默认值传入
-            Meter1.insert(cur = 1/i,curInt=i,curDouble=1/i+10,desc='g1')
-            m = Meter1(cur = 1/i,curInt=i,curDouble=1/i+10,desc='g1')
-            m.save()
-        
-        查询单条数据：
-        
-        .. code-block:: python
-        
-            #获取一条数据
-            #使用select()类方法获取查询字段（参数留空表示取全部字段），然后可以链式使用one方法获取第一条数据
-            res = Meter1.select().one()
-            print(res.desc,res.curDouble,res.curInt,res.cur,res.ts)
-        
-            #select函数中可以选择要读取的字段
-            res = Meter1.select(Meter1.cur,Meter1.desc).one()
-            print(res.desc,res.curDouble,res.curInt,res.cur,res.ts)
-        
-            #select函数中可以使用Model的类方法f()和fc()获取字符串形式的属性名与列名对应Field对象
-            res = Meter1.select(Meter1.f('cur'),Meter1.fc('c3'),Meter1.desc).one()
-            print(res.desc,res.curDouble,res.curInt,res.fc('c3'),res.f('cur'),res.ts)
-        
-        查询全部数据：
-        
-        .. code-block:: python
-        
-            #获取一条数据
-            #使用select()类方法获取查询字段（参数留空表示取全部字段），然后可以链式使用all方法获取全部数据
-            res_all = Meter1.select().all()
-            for res in res_all:
-                print(res.desc,res.curDouble,res.curInt,res.cur,res.ts)
-        
-            #select函数中可以选择要读取的字段
-            res_all = Meter1.select(Meter1.cur,Meter1.desc).all()
-            for res in res_all:
-                print(res.desc,res.curDouble,res.curInt,res.cur,res.ts)
-        
-        虽然TDengine提供了很多聚合和统计函数，但是把时序数据导入numpy或pandas等数据分析组件中进行处理的情况也是很常见的操作。
-        下面介绍如何通过crown把结果数据导入numpy和pandas
-        
-        读取数据到numpy：
-        
-        .. code-block:: python
-        
-            #通过all_raw函数可以获取二维数组格式的数据查询结果。结果每列代表的标题保存在结果对象的head属性中。
-            raw_results = Meter1.select(Meter1.cur,Meter1.curInt,Meter1.curDouble).all_raw()
-            #可以很方便的将结果转换为numpy数组对象
-            np_data = np.array(raw_results)
-            print(np_data)
-            print(raw_results.head)
-        
-        读取数据到pandas：
-        
-        .. code-block:: python
-        
-            raw_results = Meter1.select().all_raw()
-            #使用以下方法，可以轻松的将数据导入pandas,并且使用时间点作为index,使用返回的数据标题作为列名。
-            pd_data = pd.DataFrame(raw_results,columns=raw_results.head).set_index('ts')
-            print(pd_data)
-        
-        选择列四则运算：
-        
-        .. code-block:: python
-        
-            #使用select()类方法获取查询字段时，可以返回某列或多列间的值加、减、乘、除、取余计算结果（+ - * / %）
-            res_all = Meter1.select((Meter1.curDouble+Meter1.cur),Meter1.ts).all()
-            for res in res_all:
-                print(res.get(Meter1.curDouble+Meter1.cur),res.ts) #返回的结果对象可以用get方法获取原始计算式结果
-        
-            #字段别名
-            res_all = Meter1.select(((Meter1.curDouble+Meter1.cur)*Meter1.curDouble).alias('new_name'),Meter1.ts).all() #给运算式起别名（不仅运算式，其他放在select函数中的任何属性都可以使用别名）
-            for res in res_all:
-                print(res.new_name,res.ts) #使用别名获取运算结果
-        
-        where查询条件：
-        
-        .. code-block:: python
-        
-            #可以在select函数后链式调用where函数进行条件限
-            one_time =datetime.datetime.now() - datetime.timedelta(hours=10)
-            ress = Meter1.select().where(Meter1.ts > one_time).all()
-            #限定条件可以使用 > < == >= <= != and or ! 等。字符类型的字段可以使用 % 作为模糊查询（相当于like）
-            # 逻辑操作符号 |: 或 &：与 ~：非。（注意：做逻辑操作符号的表达式需要用括号括起来）
-            ress = Meter1.select().where((Meter1.cur > 0) | (Meter1.desc % 'g%')).all()
-            #where函数可以接收任意多参数，每个参数为一个限定条件，参数条件之间为"与"的关系。
-            ress = Meter1.select().where(Meter1.cur > 0, Meter1.ts > one_time, Meter1.desc % '%1').all()
-        
-        分页与limit：
-        
-        .. code-block:: python
-        
-            #可以在select函数后链式调用paginate函数进行分页操作，以下例子为取第6页 每页5条数据。
-            ress_1 = Meter1.select().paginate(6,page_size=5).all()
-            ress_2 = Meter1.select().paginate(6).all() #默认page_size为20
-            #可以在select函数后链式调用limit函数和offset函数条数限制和定位操作。
-            ress_3 = Meter1.select().limit(2).offset(5).all()
-            ress_4 = Meter1.select().limit(2).all()
-        
-        排序（目前tdengine只支持主键排序）：
-        
-        .. code-block:: python
-        
-            #可以在select函数后链式调用desc或者asc函数进行时间轴的正序或者倒序查询
-            res = Meter1.select().desc().one()
-            #定义模型类的时候定义默认排序方法
-            class Meter1(Model):
-                cur = FloatField(db_column='c1')
-                curInt = IntegerField(db_column='c2')
-                curDouble = DoubleField(db_column='c3')
-                desc = BinaryField(db_column='des')
-                dd = PrimaryKeyField().desc() #可以在定义主键的时候调用field的desc或asc方法定义默认排序
-                class Meta:
-                    # order_by= ['-dd'] #也可以在元数据类中定义‘-dd’代表倒序‘dd’ 代表正序
-                    database = db
-        
-        去重 ：
-        
-        .. code-block:: python
-        
-            #可以在select函数后链式调用distinct函数对返回的数据列进行去重复操作
-            res = Meter1.select().distinct().all()
-        
-        聚合函数：
-        
-        .. code-block:: python
-        
-            #count
-            count = Meter1.select().count() #统计行数
-            print(count) # 结果： 100
-            count = Meter1.select().count(Meter1.desc) #统计指定列非空行数
-            print(count) # 结果： 90
-            #avg（sum,stddev,min,max,first,last,last_row,spread使用方法与avg相同）
-            avg1 = Meter1.select().avg(Meter1.cur,Meter1.curDouble.alias('aa')) #可以同时获取多列，并且可以使用别名
-            print(avg1.get(Meter1.cur.avg()),avg1.aa) #打印统计结果
-            #twa 必须配合where函数，且必须选择时间段
-            twa1 = Meter1.select().where(Meter1.ts > datetime.datetime(2020, 11, 19, 15, 9, 12, 946118),Meter1.ts < datetime.datetime.now()).twa(Meter1.cur,Meter1.curDouble.alias('aa'))
-            print(twa1.get(Meter1.cur.twa()),avg1.aa) #打印统计结果
-        
-            #diff
-            diffs = Meter1.select().diff(Meter1.curInt.alias('aa')) #diff目前只可以聚合一个属性。
-            for diff1 in diffs:
-                print(diff1.aa,diff1.ts) # 时间点数据同时返回
-        
-            #top(bottom函数使用方式相同)
-            tops = Meter1.select().top(Meter1.cur,3,alias='aa') # top函数需要提供要统计的属性，行数，以及别名
-            for top1 in tops:
-                print(top1.aa,top1.ts) # 时间点数据同时返回
-            tops = Meter1.select().top(Meter1.cur,3) # 可以不指定别名
-            for top1 in tops:
-                print(top1.get(Meter1.cur.top(3))) #不指定别名，需用使用get方法获取属性
-        
-            #percentile (apercentile函数使用方式相同) 
-            percentile1 = Meter1.select().percentile((Meter1.cur,1,'aa'),(Meter1.curDouble,2)) #每个属性参数为一个元组（数组），分别定义要统计的属性，P值（P值取值范围0≤P≤100），可选别名。
-            print(percentile1.aa)
-            print(percentile1.get(Meter1.curDouble.percentile(2)))#不指定别名，需用使用get方法获取属性
-        
-            #leastsquares
-            leastsquares1 = Meter1.select().leastsquares((Meter1.cur,1,1,'aa'),(Meter1.curDouble,2,2)) #每个属性参数为一个元组（数组），分别定义要统计的属性，start_val(自变量初始值)，step_val(自变量的步长值)，可选别名。
-            print(leastsquares1.aa) # 结果： {slop:-0.001595, intercept:0.212111}
-            print(leastsquares1.get(Meter1.curDouble.leastsquares(2,2))) #不指定别名，需用使用get方法获取属性
-        
-        group_by分组查询：
-        
-        .. code-block:: python
-        
-            # 可以在链式调用中加入group_by函数指定要分组的字段。然后在select函数中指定要分组统计的聚合函数（支持的聚合函数有：count、avg、sum 、stddev、leastsquares、percentile、min、max、first、last）
-            groups= Meter1.select(Meter1.desc,Meter1.curInt.avg().alias('intavg'),Meter1.cur.count().alias('curcount')).group_by(Meter1.desc).all()
-            for group in groups:
-                print(group.desc)
-                if group.desc == 'g1':
-                    # assert group.get(Meter1.curInt.count()) == 10
-                    assert group.intavg == 5.5
-                    assert group.curcount == 10
-                if group.desc == 'g2':
-                    assert group.intavg == 10.5
-                    assert group.curcount == 20
-        
-        时间维度聚合interval:
-        
-        .. code-block:: python
-        
-            # 可以使用interval函数调用TDengine时间纬度聚合功能,使用方法如下 时间间隔与offset参数参考TDengine文档（s:秒，m:分钟，h:小时）。fill参数可选字符串(NONE | PREV | NULL | LINEAR)或者任意数值,例如：fill=1.2将会以固定值填充。
-            results= Meter1.select(Meter1.cur.avg().alias('aa'),Meter1.cur.first().alias('bb')).where(Meter1.ts > (datetime.datetime.now()-datetime.timedelta(days=1))).interval('10s',fill='PREV',offset='1m').all()
-            for result in results:
-                print(result.aa,result.bb)
-        
-        join查询：
-        
-        目前并支持多表join查询，需要多表查询的情况请使用raw_sql函数，执行原始sql语句。以后的版本会补充此功能。
-        
-        
-        超级表定义：
-        
-        .. code-block:: python
-        
-            # 超级表模型类继承自SuperModel类
-            class Meters(SuperModel):
-                cur = FloatField(db_column='c1')
-                curInt = IntegerField(db_column='c2')
-                curDouble = DoubleField(db_column='c3')
-                desc = BinaryField(db_column='des')
-                class Meta:
-                    database = db
-                    db_table = 'meters'
-                    # Meta类中定义的Field，为超级表的标签
-                    location = BinaryField(max_length=30)
-                    groupid = IntegerField(db_column='gid')
-        
-        超级表的建表、删表、检查表是否存在：
-        
-        .. code-block:: python
-        
-            Meters.create_table(safe=True) #建表 safe：如果表存在，则跳过建表指令。命令运行成功放回True,失败raise错误
-            # db.create_table(Meters,safe=True) #通过数据库对象建表，功能同上
-            Meters.drop_table(safe=True) #删表 safe：如果表不存在，则跳过删表指令。命令运行成功放回True,失败raise错误
-            # db.drop_table(Meters,safe=True) #通过数据库对象删表，功能同上
-            Meters.supertable_exists() #查看表是否存在，存在返回True,不存在返回：False
-        
-        超级表动态建表：
-        
-        超级表除了使用定义模型类的方式建表外，也提供了动态定义字段建表的功能。
-        
-        .. code-block:: python
-        
-            #可以使用SuperModel类的类方法dynamic_create_table方法动态建表，第一个参数为表名，然后需要指定数据库，与是否安全建表
-            # 需要额外提供tags参数，参数值为一个字典(使用方法如下例)，设置超级表所有的标签。
-            # 关键词参数可以任意多个，指定表中的字段。
-            Meter_dynamic= SuperModel.dynamic_create_table('meterSD',database=db,safe=True,tags={'gid':IntegerField(db_column='tag1')},test1 = FloatField(db_column='t1'),test2 = IntegerField(db_column='t2'))
-            # 函数返回的对象为SuperModel类对象。使用方法与静态继承的模型类相同。
-            Meter_dynamic.supertable_exists()
-            Meter_dynamic.drop_table()
-        
-        从表名建立对应的supermodel类：
-        
-        数据库中已有的数据库超级表，可以通过已知的表名建立对应的supermodel类。
-        
-        .. code-block:: python
-        
-            sTable = SuperModel.supermodel_from_table('rule_10',db) # rule_10为数据表的表名
-            res = sTable.select().one() # 从表名新建的类和静态建立的类，使用方法完全一致
-        
-        从超级表建立子表：
-        
-        .. code-block:: python
-        
-            SonTable_d3 = Meters.create_son_table('d3',location='beijing',groupid=3) #生成字表模型类的同时，自动在数据库中建表。
-        
-            SonTable_d3.table_exists() # SonTable_d3的使用方法和继承自Modle类的模型类一样。可以进行插入与查询操作
-            # m = SonTable_d3(cur = 65.8,curInt=10,curDouble=1.1,desc='g1',ts = datetime.datetime.now())
-            # m.save()
-        
-        新增标签：
-        
-        .. code-block:: python
-        
-            # 使用add_tags方法，可以给超级表新建多个标签。每个参数可以是一个Field对象（必须指定db_column属性）
-            Meters.add_tags(IntegerField(db_column='add_tag_1'),IntegerField(db_column='add_tag_4'),BinaryField(max_length=30,db_column='add_tag_5'))
-        
-        删除标签：
-        
-        .. code-block:: python
-        
-            # 使用drop_tag方法可以删除超级表的标签，参数名为标签名，一次只能删除一个标签
-            Meters.drop_tag('add_tag_2')
-        
-        修改标签名：
-        
-        .. code-block:: python
-        
-            # 使用change_tag_name方法可以修改超级表的标签名，参数名为要修改的标签名，和新的标签名。（注意：此方法只修改对应超级表的标签名，并不修改类的属性名）
-            Meters.change_tag_name('add_tag_1','add_tag_2')
-        
-        
-        修改子表标签值：
-        
-        .. code-block:: python
-        
-            TableT = Meters.create_son_table('d3_insert',location='beijing',gid=3)
-            # 子表可以通过change_tag_value方法修改自己的标签值。
-            TableT.change_tag_value(location='tianjin',gid = 6)
-        
-        
-        
-        关于debug信息打印：
-        
-        如需查看crown调用tdengine引擎时执行的sql语句和返回的原始数据。只需要配置crown模块的logger记录器的日志输出级别为debug即可。
-        
-        .. code-block:: python
-        
-            import logging
-            from crown import logger
-        
-            logger.setLevel(logging.DEBUG) #配置logger对象，即可输出执行debug信息
-        
 Keywords: orm,taos,TDengine,TSDB,Time Series Database,connector,python
-Platform: UNKNOWN
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+crown
+======
+
+crown 是一个轻量级的针对时序数据（TSDB）TDengine的ORM库。 
+
+* 需要python 3.0版本以上
+* 0.1.7版本在tdengine 2版本测试通过
+* 0.3.0版本在tdengine 3版本测试通过
+* 解决mac操作系统下没有原生python连接器的问题
+* 极大的降低了python程序员使用TDengine技术门槛
+* 可以方便的将数据转换到numpy与pandas
+* 目前使用TDengine的restful接口连接数据库，以后将提供原生接口引擎可供选择（目前原生接口无法在mac系统上使用）
+
+安装
+----------------------
+
+大多数情况下，可以通过pip,轻松安装最新版本：
+
+.. code-block:: console
+
+    pip install crown
+
+
+还可以通过git安装，项目地址： https://github.com/machine-w/crown
+
+使用方法:
+
+.. code-block:: console
+
+    git clone https://github.com/machine-w/crown.git
+    cd crowm
+    python setup.py install
+
+
+使用文档
+------------------------
+
+建立数据库与删除数据库:
+
+.. code-block:: python
+
+    from crown import *
+
+    DATABASENAME = 'taos_test'
+    HOST = 'localhost'
+    PORT = 6041
+    # 默认端口 6041，默认用户名：root,默认密码：taosdata
+    db = TdEngineDatabase(DATABASENAME,host=HOST) #新建数据库对象
+    # db.connect()  # 尝试连接数据库，如果库不存在，则自动建库。
+    # print(db.databases) #连接数据库db对象后会自动获取全部数据库信息，以字典的形式保存在属性databases中。
+    # 如不使用默认值，可以如下传入参数
+    # db = TdEngineDatabase(DATABASENAME,host=HOST,port=PORT,user='yourusername',passwd='yourpassword')
+    db.create_database(safe=True)  #建库指令。 （safe：如果库存在，则跳过建库指令。）
+    # db.create_database(safe=True,keep= 100,comp=0,replica=1,quorum=2,blocks=115) #可选字段：建库时配置数据库参数，具体字段含义请参考tdengine文档。
+    db.drop_database(safe=True) #删库指令 （safe：如果库不存在，则跳过删库指令。）
+
+修改数据库参数:
+
+.. code-block:: python
+
+    db.alter_database(keep= 120,comp=1,replica=1,quorum=1,blocks=156) #同建库可选字段。
+
+执行sql语句:
+
+.. code-block:: python
+
+    #可以通过数据库对象直接执行sql语句，语句规则与TDengine restful接口要求一致。
+    res = db.raw_sql('select c1,c2 from taos_test.member1')
+    print(res,res.head,res.rowcount) #返回的对象为二维数据。res.head属性为数组对象，保存每一行数据的代表的列名。res.rowcount属性保存返回行数。
+    # res: [[1.2,2.2],[1.3,2.1],[1.5,2.0],[1.6,2.1]]
+    # res.head: ['c1','c2']
+    # res.rowcount: 4
+
+打印执行的sql语句:
+
+.. code-block:: python
+
+    Meter1.select().one()
+    print(db.curSql) #可以通过db对象的curSql属性获取当前执行的原始sql语句
+
+模型定义:
+
+.. code-block:: python
+
+    from crown import *
+
+    DATABASENAME = 'taos_test'
+    HOST = 'localhost'
+    db = TdEngineDatabase(DATABASENAME,host=HOST) #新建数据库对象
+    db.connect()  #尝试连接数据库，如果库不存在，则自动建库。
+    # print(db.databases) #连接数据库db对象后会自动获取全部数据库信息，以字典的形式保存在属性databases中。
+
+    # 表模型类继承自Model类，每个模型类对应数据库中的一张表，模型类中定义的每个Field，对应表中的一列
+    class Meter1(Model):
+        cur = FloatField(db_column='c1')
+        curInt = IntegerField(db_column='c2')
+        curDouble = DoubleField(db_column='c3')
+        desc = BinaryField(db_column='des')
+
+        class Meta: #Meta子类中定义模型类的配置信息
+            database = db #指定表所使用的数据库
+            db_table = 'meter1' #指定表名
+
+    # 可选择的全部Field类型如下，类型与Tdengine支持的数据类型一一对应
+    class AllField(Model):
+        name_float = FloatField(column_name='nf1') #可选项：指定列名
+        name_double = DoubleField()
+        name_bigint = BigIntegerField()
+        name_int = IntegerField()
+        name_smallint = SmallIntegerField()
+        name_tinyint = TinyIntegerField()
+        name_nchar = NCharField(max_length=59,db_column='n1')
+        name_binary = BinaryField(max_length=3)
+        name_bool = BooleanField()
+        dd = PrimaryKeyField() # 如果定义了主键列，则使用主键列作为主键，如果没有定义，则默认“ts”为主键。
+        birthday = DateTimeField()
+        class Meta:
+            database = db
+            db_table = 'all_field'
+
+主键定义：
+
+.. code-block:: python
+
+    #定义主键方式1 
+    #不定义主键，系统默认主键：“ts”
+    class TestPri(Model):
+        cur = FloatField(db_column='c1')
+        class Meta:
+            database = db
+    res = TestPri.describe_table() #获取表结构信息
+    print(res[0][0]) # 结果: “ts”
+
+    #定义主键方式2
+    class TestPri(Model):
+        cur = FloatField(db_column='c1')
+        timeline = PrimaryKeyField() #定义主键列，主键名设置为列名
+        class Meta:
+            database = db
+    res = TestPri.describe_table()
+    print(res[0][0]) # 结果: “timeline”
+
+     #定义主键方式3
+    class TestPri(Model):
+        cur = FloatField(db_column='c1')
+        class Meta:
+            database = db
+            primary_key = 'timeline' # Meta中定主键名称
+    res = TestPri.describe_table()
+    print(res[0][0]) # 结果: “timeline”
+    
+
+
+建表、删表、检查表是否存在：
+
+.. code-block:: python
+
+    Meter1.create_table(safe=True) #建表 safe：如果表存在，则跳过建表指令。命令运行成功放回True,失败raise错误
+    # db.create_table(Meter1,safe=True) #通过数据库对象建表，功能同上
+    Meter1.drop_table(safe=True) #删表 safe：如果表不存在，则跳过删表指令。命令运行成功放回True,失败raise错误
+    # db.drop_table(Meter1,safe=True) #通过数据库对象删表，功能同上
+    Meter1.table_exists() #查看表是否存在，存在返回True,不存在返回：False
+
+动态建表：
+
+除了使用定义模型类的方式建表外，还提供了动态定义字段建表的功能。
+
+.. code-block:: python
+
+    #可以使用Model类的类方法dynamic_create_table方法动态建表，第一个参数为表名，然后需要指定数据库，与是否安全建表。
+    # 关键词参数可以任意多个，指定表中的字段。
+    Meter_dynamic= Model.dynamic_create_table('meterD',database=db,safe=True,test1 = FloatField(db_column='t1'),test2 = IntegerField(db_column='t2'))
+    # 函数返回的对象为Model类对象。使用方法与静态继承的模型类相同。
+    Meter_dynamic.table_exists()
+    Meter_dynamic.drop_table()
+
+从表名建立对应的model类：
+
+数据库中已有的数据库表，可以通过已知的表名建立对应的model类。
+
+.. code-block:: python
+
+    nodeTable = Model.model_from_table('node_10',db) # node_10为数据表的表名
+    res = nodeTable.select().one() # 从表名新建的类和静态建立的类，使用方法完全一致
+    
+    
+动态建立的或从数据库分析得到的model对象，可以直接使用列名作为属性名进行查询操作。
+
+.. code-block:: python
+
+
+    res = nodeTable.select(nodeTable.c1)where(nodeTable.c1 > 1).all() # 直接使用列名
+    res = nodeTable.select(nodeTable.c1)where(FloatField(db_column='c1') > 1).all() # 也可以使用field对象作为字段检索条件（多使用于列名为动态值的时候）
+    # 直接使用列名,查看结果
+    for item in res:
+        print(item.c1)
+
+插入数据：
+
+.. code-block:: python
+
+    #方法一
+    for i in range(1,101):
+        #使用模型类实例化的每个对象对应数据表中的每一行，可以通过传入属性参数的方式给每一列赋值
+        m = Meter1(cur = 1/i,curInt=i,curDouble=1/i+10,desc='g1',ts= datetime.datetime.now() - datetime.timedelta(seconds=(102-i)))
+        #使用对象的save方法将数据存入数据库
+        m.save()
+    print(Meter1.select().count()) # 结果：100
+    #方法二
+    for i in range(1,11):
+        #也可以直接使用模型类的insert方法插入数据。
+        Meter1.insert(cur = 1/i,curInt=i,curDouble=1/i+10,desc='g1',ts= datetime.datetime.now() - datetime.timedelta(seconds=(12-i)))
+    print(Meter1.select().count()) # 结果：100
+    #如果不传入时间属性，则会以当前时刻为默认值传入
+    Meter1.insert(cur = 1/i,curInt=i,curDouble=1/i+10,desc='g1')
+    m = Meter1(cur = 1/i,curInt=i,curDouble=1/i+10,desc='g1')
+    m.save()
+
+查询单条数据：
+
+.. code-block:: python
+
+    #获取一条数据
+    #使用select()类方法获取查询字段（参数留空表示取全部字段），然后可以链式使用one方法获取第一条数据
+    res = Meter1.select().one()
+    print(res.desc,res.curDouble,res.curInt,res.cur,res.ts)
+
+    #select函数中可以选择要读取的字段
+    res = Meter1.select(Meter1.cur,Meter1.desc).one()
+    print(res.desc,res.curDouble,res.curInt,res.cur,res.ts)
+
+    #select函数中可以使用Model的类方法f()和fc()获取字符串形式的属性名与列名对应Field对象
+    res = Meter1.select(Meter1.f('cur'),Meter1.fc('c3'),Meter1.desc).one()
+    print(res.desc,res.curDouble,res.curInt,res.fc('c3'),res.f('cur'),res.ts)
+
+查询全部数据：
+
+.. code-block:: python
+
+    #获取一条数据
+    #使用select()类方法获取查询字段（参数留空表示取全部字段），然后可以链式使用all方法获取全部数据
+    res_all = Meter1.select().all()
+    for res in res_all:
+        print(res.desc,res.curDouble,res.curInt,res.cur,res.ts)
+
+    #select函数中可以选择要读取的字段
+    res_all = Meter1.select(Meter1.cur,Meter1.desc).all()
+    for res in res_all:
+        print(res.desc,res.curDouble,res.curInt,res.cur,res.ts)
+
+虽然TDengine提供了很多聚合和统计函数，但是把时序数据导入numpy或pandas等数据分析组件中进行处理的情况也是很常见的操作。
+下面介绍如何通过crown把结果数据导入numpy和pandas
+
+读取数据到numpy：
+
+.. code-block:: python
+
+    #通过all_raw函数可以获取二维数组格式的数据查询结果。结果每列代表的标题保存在结果对象的head属性中。
+    raw_results = Meter1.select(Meter1.cur,Meter1.curInt,Meter1.curDouble).all_raw()
+    #可以很方便的将结果转换为numpy数组对象
+    np_data = np.array(raw_results)
+    print(np_data)
+    print(raw_results.head)
+
+读取数据到pandas：
+
+.. code-block:: python
+
+    raw_results = Meter1.select().all_raw()
+    #使用以下方法，可以轻松的将数据导入pandas,并且使用时间点作为index,使用返回的数据标题作为列名。
+    pd_data = pd.DataFrame(raw_results,columns=raw_results.head).set_index('ts')
+    print(pd_data)
+
+选择列四则运算：
+
+.. code-block:: python
+
+    #使用select()类方法获取查询字段时，可以返回某列或多列间的值加、减、乘、除、取余计算结果（+ - * / %）
+    res_all = Meter1.select((Meter1.curDouble+Meter1.cur),Meter1.ts).all()
+    for res in res_all:
+        print(res.get(Meter1.curDouble+Meter1.cur),res.ts) #返回的结果对象可以用get方法获取原始计算式结果
+
+    #字段别名
+    res_all = Meter1.select(((Meter1.curDouble+Meter1.cur)*Meter1.curDouble).alias('new_name'),Meter1.ts).all() #给运算式起别名（不仅运算式，其他放在select函数中的任何属性都可以使用别名）
+    for res in res_all:
+        print(res.new_name,res.ts) #使用别名获取运算结果
+
+where查询条件：
+
+.. code-block:: python
+
+    #可以在select函数后链式调用where函数进行条件限
+    one_time =datetime.datetime.now() - datetime.timedelta(hours=10)
+    ress = Meter1.select().where(Meter1.ts > one_time).all()
+    #限定条件可以使用 > < == >= <= != and or ! 等。字符类型的字段可以使用 % 作为模糊查询（相当于like）
+    # 逻辑操作符号 |: 或 &：与 ~：非。（注意：做逻辑操作符号的表达式需要用括号括起来）
+    ress = Meter1.select().where((Meter1.cur > 0) | (Meter1.desc % 'g%')).all()
+    #where函数可以接收任意多参数，每个参数为一个限定条件，参数条件之间为"与"的关系。
+    ress = Meter1.select().where(Meter1.cur > 0, Meter1.ts > one_time, Meter1.desc % '%1').all()
+
+分页与limit：
+
+.. code-block:: python
+
+    #可以在select函数后链式调用paginate函数进行分页操作，以下例子为取第6页 每页5条数据。
+    ress_1 = Meter1.select().paginate(6,page_size=5).all()
+    ress_2 = Meter1.select().paginate(6).all() #默认page_size为20
+    #可以在select函数后链式调用limit函数和offset函数条数限制和定位操作。
+    ress_3 = Meter1.select().limit(2).offset(5).all()
+    ress_4 = Meter1.select().limit(2).all()
+
+排序（目前tdengine只支持主键排序）：
+
+.. code-block:: python
+
+    #可以在select函数后链式调用desc或者asc函数进行时间轴的正序或者倒序查询
+    res = Meter1.select().desc().one()
+    #定义模型类的时候定义默认排序方法
+    class Meter1(Model):
+        cur = FloatField(db_column='c1')
+        curInt = IntegerField(db_column='c2')
+        curDouble = DoubleField(db_column='c3')
+        desc = BinaryField(db_column='des')
+        dd = PrimaryKeyField().desc() #可以在定义主键的时候调用field的desc或asc方法定义默认排序
+        class Meta:
+            # order_by= ['-dd'] #也可以在元数据类中定义‘-dd’代表倒序‘dd’ 代表正序
+            database = db
+
+去重 ：
+
+.. code-block:: python
+
+    #可以在select函数后链式调用distinct函数对返回的数据列进行去重复操作
+    res = Meter1.select().distinct().all()
+
+聚合函数：
+
+.. code-block:: python
+
+    #count
+    count = Meter1.select().count() #统计行数
+    print(count) # 结果： 100
+    count = Meter1.select().count(Meter1.desc) #统计指定列非空行数
+    print(count) # 结果： 90
+    #avg（sum,stddev,min,max,first,last,last_row,spread使用方法与avg相同）
+    avg1 = Meter1.select().avg(Meter1.cur,Meter1.curDouble.alias('aa')) #可以同时获取多列，并且可以使用别名
+    print(avg1.get(Meter1.cur.avg()),avg1.aa) #打印统计结果
+    #twa 必须配合where函数，且必须选择时间段
+    twa1 = Meter1.select().where(Meter1.ts > datetime.datetime(2020, 11, 19, 15, 9, 12, 946118),Meter1.ts < datetime.datetime.now()).twa(Meter1.cur,Meter1.curDouble.alias('aa'))
+    print(twa1.get(Meter1.cur.twa()),avg1.aa) #打印统计结果
+
+    #diff
+    diffs = Meter1.select().diff(Meter1.curInt.alias('aa')) #diff目前只可以聚合一个属性。
+    for diff1 in diffs:
+        print(diff1.aa,diff1.ts) # 时间点数据同时返回
+
+    #top(bottom函数使用方式相同)
+    tops = Meter1.select().top(Meter1.cur,3,alias='aa') # top函数需要提供要统计的属性，行数，以及别名
+    for top1 in tops:
+        print(top1.aa,top1.ts) # 时间点数据同时返回
+    tops = Meter1.select().top(Meter1.cur,3) # 可以不指定别名
+    for top1 in tops:
+        print(top1.get(Meter1.cur.top(3))) #不指定别名，需用使用get方法获取属性
+
+    #percentile (apercentile函数使用方式相同) 
+    percentile1 = Meter1.select().percentile((Meter1.cur,1,'aa'),(Meter1.curDouble,2)) #每个属性参数为一个元组（数组），分别定义要统计的属性，P值（P值取值范围0≤P≤100），可选别名。
+    print(percentile1.aa)
+    print(percentile1.get(Meter1.curDouble.percentile(2)))#不指定别名，需用使用get方法获取属性
+
+    #leastsquares
+    leastsquares1 = Meter1.select().leastsquares((Meter1.cur,1,1,'aa'),(Meter1.curDouble,2,2)) #每个属性参数为一个元组（数组），分别定义要统计的属性，start_val(自变量初始值)，step_val(自变量的步长值)，可选别名。
+    print(leastsquares1.aa) # 结果： {slop:-0.001595, intercept:0.212111}
+    print(leastsquares1.get(Meter1.curDouble.leastsquares(2,2))) #不指定别名，需用使用get方法获取属性
+
+group_by分组查询：
+
+.. code-block:: python
+
+    # 可以在链式调用中加入group_by函数指定要分组的字段。然后在select函数中指定要分组统计的聚合函数（支持的聚合函数有：count、avg、sum 、stddev、leastsquares、percentile、min、max、first、last）
+    groups= Meter1.select(Meter1.desc,Meter1.curInt.avg().alias('intavg'),Meter1.cur.count().alias('curcount')).group_by(Meter1.desc).all()
+    for group in groups:
+        print(group.desc)
+        if group.desc == 'g1':
+            # assert group.get(Meter1.curInt.count()) == 10
+            assert group.intavg == 5.5
+            assert group.curcount == 10
+        if group.desc == 'g2':
+            assert group.intavg == 10.5
+            assert group.curcount == 20
+
+时间维度聚合interval:
+
+.. code-block:: python
+
+    # 可以使用interval函数调用TDengine时间纬度聚合功能,使用方法如下 时间间隔与offset参数参考TDengine文档（s:秒，m:分钟，h:小时）。fill参数可选字符串(NONE | PREV | NULL | LINEAR)或者任意数值,例如：fill=1.2将会以固定值填充。
+    results= Meter1.select(Meter1.cur.avg().alias('aa'),Meter1.cur.first().alias('bb')).where(Meter1.ts > (datetime.datetime.now()-datetime.timedelta(days=1))).interval('10s',fill='PREV',offset='1m').all()
+    for result in results:
+        print(result.aa,result.bb)
+
+join查询：
+
+目前并支持多表join查询，需要多表查询的情况请使用raw_sql函数，执行原始sql语句。以后的版本会补充此功能。
+
+
+超级表定义：
+
+.. code-block:: python
+
+    # 超级表模型类继承自SuperModel类
+    class Meters(SuperModel):
+        cur = FloatField(db_column='c1')
+        curInt = IntegerField(db_column='c2')
+        curDouble = DoubleField(db_column='c3')
+        desc = BinaryField(db_column='des')
+        class Meta:
+            database = db
+            db_table = 'meters'
+            # Meta类中定义的Field，为超级表的标签
+            location = BinaryField(max_length=30)
+            groupid = IntegerField(db_column='gid')
+
+超级表的建表、删表、检查表是否存在：
+
+.. code-block:: python
+
+    Meters.create_table(safe=True) #建表 safe：如果表存在，则跳过建表指令。命令运行成功放回True,失败raise错误
+    # db.create_table(Meters,safe=True) #通过数据库对象建表，功能同上
+    Meters.drop_table(safe=True) #删表 safe：如果表不存在，则跳过删表指令。命令运行成功放回True,失败raise错误
+    # db.drop_table(Meters,safe=True) #通过数据库对象删表，功能同上
+    Meters.supertable_exists() #查看表是否存在，存在返回True,不存在返回：False
+
+超级表动态建表：
+
+超级表除了使用定义模型类的方式建表外，也提供了动态定义字段建表的功能。
+
+.. code-block:: python
+
+    #可以使用SuperModel类的类方法dynamic_create_table方法动态建表，第一个参数为表名，然后需要指定数据库，与是否安全建表
+    # 需要额外提供tags参数，参数值为一个字典(使用方法如下例)，设置超级表所有的标签。
+    # 关键词参数可以任意多个，指定表中的字段。
+    Meter_dynamic= SuperModel.dynamic_create_table('meterSD',database=db,safe=True,tags={'gid':IntegerField(db_column='tag1')},test1 = FloatField(db_column='t1'),test2 = IntegerField(db_column='t2'))
+    # 函数返回的对象为SuperModel类对象。使用方法与静态继承的模型类相同。
+    Meter_dynamic.supertable_exists()
+    Meter_dynamic.drop_table()
+
+从表名建立对应的supermodel类：
+
+数据库中已有的数据库超级表，可以通过已知的表名建立对应的supermodel类。
+
+.. code-block:: python
+
+    sTable = SuperModel.supermodel_from_table('rule_10',db) # rule_10为数据表的表名
+    res = sTable.select().one() # 从表名新建的类和静态建立的类，使用方法完全一致
+
+从超级表建立子表：
+
+.. code-block:: python
+
+    SonTable_d3 = Meters.create_son_table('d3',location='beijing',groupid=3) #生成字表模型类的同时，自动在数据库中建表。
+
+    SonTable_d3.table_exists() # SonTable_d3的使用方法和继承自Modle类的模型类一样。可以进行插入与查询操作
+    # m = SonTable_d3(cur = 65.8,curInt=10,curDouble=1.1,desc='g1',ts = datetime.datetime.now())
+    # m.save()
+
+新增标签：
+
+.. code-block:: python
+
+    # 使用add_tags方法，可以给超级表新建多个标签。每个参数可以是一个Field对象（必须指定db_column属性）
+    Meters.add_tags(IntegerField(db_column='add_tag_1'),IntegerField(db_column='add_tag_4'),BinaryField(max_length=30,db_column='add_tag_5'))
+
+删除标签：
+
+.. code-block:: python
+
+    # 使用drop_tag方法可以删除超级表的标签，参数名为标签名，一次只能删除一个标签
+    Meters.drop_tag('add_tag_2')
+
+修改标签名：
+
+.. code-block:: python
+
+    # 使用change_tag_name方法可以修改超级表的标签名，参数名为要修改的标签名，和新的标签名。（注意：此方法只修改对应超级表的标签名，并不修改类的属性名）
+    Meters.change_tag_name('add_tag_1','add_tag_2')
+
+
+修改子表标签值：
+
+.. code-block:: python
+
+    TableT = Meters.create_son_table('d3_insert',location='beijing',gid=3)
+    # 子表可以通过change_tag_value方法修改自己的标签值。
+    TableT.change_tag_value(location='tianjin',gid = 6)
+
+
+
+关于debug信息打印：
+
+如需查看crown调用tdengine引擎时执行的sql语句和返回的原始数据。只需要配置crown模块的logger记录器的日志输出级别为debug即可。
+
+.. code-block:: python
+
+    import logging
+    from crown import logger
+
+    logger.setLevel(logging.DEBUG) #配置logger对象，即可输出执行debug信息
```

### Comparing `crown-0.1.7/setup.py` & `crown-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     packages=['crown'],
     description="crown is a simple and small ORM for Time Series Database (TSDB) tdengine(taos), making it easy to learn and intuitive to use.",
     long_description=README,
     long_description_content_type='text/markdown',
     install_requires=[
         'requests>=2.23.0'
     ],
-    version='0.1.7',
+    version='0.3.0',
     url='https://github.com/machine-w/crown',
     author='machine-w',
     author_email='steve2008.ma@gmail.com',
     keywords=['orm','taos', 'TDengine', 'TSDB','Time Series Database','connector','python'],
     tests_require=[
         'pytest',
         'pytest-faker',
```

