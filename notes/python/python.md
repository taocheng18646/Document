通过解释器运行python
	Python 路劲和文件名
### 2.python基础语法
	数据类型
	字符串要用双引号包围起来
	注释： # 和内容用空格隔开
	“”“”“”“ 多行注释，三个引号
	传输变量
		Money=5-
		print（money）s
		输出 ：50 
		可以直接传参数
	2.2验证数据类型（内置函数）
		Type("sfhsfk")
		也可以将这些内置函数进行赋值
		Type_1 = type(""lsjfjlsf""）
		print（type_1)
		变量没有类型，变量存储的数据有类型
	2.3数据类型转换
		Int(x) 将x转换为整数
		Float(x)
		Str(x)
	2.4标识符
		大小写完全区分
		不可使用关键字
		不能以数字开头
		命名规则
			见名知意
			下划线命名
			英文字母全小写
	2.5运算符
		算术运算符我 + - * /
		取证 //  取余% 指数**
		Num +=1  # num = num +1
	2.6字符串扩展
		1、三种定义方法
			单引号 双引号 三引号
			字符串本身包含引号
				单引号内包含双引号  双引号内包含单引号  \转义字符使其变成普通字
		2、字符串拼接（不同类型的数据可能不能拼接）只能用于字符串本身
			一般用于变量和变量进行拼接
			用+号即可
		3、字符串格式化(和其他类型拼接）
			 name = "小明"
			 message = "您好 %s" %name
			%表示占位 S表示将变量变成字符串放入占位地方
			多变量占位，% （var1，var2）变量顺序不能变
			三类占位
				%s 将内容转换成字符串
				%d将内容转换成整数
				%f将内容转换成浮点数
		4、格式化中对数字的精度控制
			用m.n来控制数据的宽度和精度
			例如
				%5.2f表示整数和小数的宽度为5，不足5为补空格，小数两位，四舍五入
		5、字符串格式化方式2（适合对精度没有要求的数据类型）
			通过%占位已经很方便了，还有更好的占位以及控制宽度和精度的方法
			f“{varname}”
			print（f”我是一个{var1}，今年{var2}岁”）
			用f直接声明要进行占位，同时不做精度控制，输出原样
		6、对表达式进行格式化
			表达式：一条具有明确执行结果的代码语句，有具体结果
			例如
				prin他（“shfhsfh%s” % （1+1）
				表达式直接传入到占位符当中
	2.7数据输入
		数据输入 input
			Name = input("提示信息")
			转数字类型
			Name = int(num)
			Num=int（input（”请输入您的年龄“）#转化为整形
3.判断语句
	布尔类型：True（1）   False（0）
	定义变量：变量名称=布尔类型字面量
	比较运算符 ==是否相等
			！=不等于
	3.2判断语句
		if语句
			If 条件：（引号）
				（四个空格缩进）条件成立时，要做的事情
			判断语句的结果必须是布尔类型
			True会执行
			false不执行
		
		If else组合（不满足可供执行的代码）
			If 条件：
				满足程序
			esle：
				不满足程序
		注意：冒号，缩进
		
		If elif esle组合语句
			If 条件：
			elif条件：
			elif条件：
			else：（都不满足后执行）
		从上到下执行，第一个满足，后面都不执行
	3.3判断语句嵌套
		外层，内层，九九乘法表
4.循环语句
	4.1while循环
		i=0
		Whlie i<100:
			Print("这里是程序"）
			i+=1
		注意循环条件和循环程序
		不能无限循环
		需要设置终止条件
		\t制表符，可以让我们多行输出对齐
		若前面没有字符串，则补齐8个，若前面有三个字符串则补齐5个空格，这是补齐到8的倍数
		确保print不换行
			Print(   , end = ' ')加入end等于空格即可
	4.2for循环
		本质上是遍历，序列类型
		while循环的循环条件是自定义，自行控制循环条件
		for循环是一种轮询机制，是对一批内容进行逐个处理
		是将待办事项，逐个完成
		For 临时变量 in 待处理数据集：
			循环程序
		同whlie循环不同，for循环是无法定义循环条件的
		只能从被处理的数据集中，依次取出内容进行处理
	4.3range类型
		语法：
			range（num）
			range（5） 取值 0 1 2 3 4 5
			range（num1，num2）不包含num2本省
			range（num1，num2，step）
	4.4for循环变量临时作用域
		For I in range(5):
			Print(i)
		Print(i) #能否访问到i？
		实际上可以访问到临时变量i，但是规范上不允许，实际操作不建议
		注意缩进
	4.5continue 和 break
		用以对循环进行临时跳过或中断
		For I in range（5）：
			语句1
			Continue
			语句2
		执行语句1之后，执行continue ，结束本次循环，开始下一次循环，语句2不执行
		break直接结束整个循环语句，不再进行下一轮循环
		break和continue都是只对其所在的循环生效，不对嵌套的外层循环生效

5函数
	5.1函数的定义
		def函数名（传入参数）：
			函数体
			return返回值
		函数调用：
			函数名（参数）
		注意：
			参数可以省略
			返回值可以省略
			必须先定义后使用
	5.3函数的参数
		传入参数的时候，调用参数也需要按照顺序进行传入参数
		定义时叫做形参
		调用时称为实参
		参数用逗号进行分离（x,y)
	5.4返回值
		主要是为了让函数执行结果返回给调用者一个结果，其实这个结果可以更好地当作一个参数使用
		例如：
			Def add (a,b):
				Result=a+b
				Return result
			r=add(1,2)
			Print（r）这样就把函数结果以参数的形式传递给了r
			其中函数体遇到return之后，后面的所有程序都不会执行，已经结束了，不要把代码写到ruturn之后
	5.5函数返回值的none类型
		无返回值的函数，本质上就是返回了None这个类型
		例如：Def add (a,b):
				Result=a+b
			R = add(1,3),返回值为none
			if判断中，none等同于false
	5.6函数说明
		Def fun(x,y):
			"""
			函数说明
			：parm x
			：parm y
			：return
			”“”
	5.7函数嵌套调用
		Def 函数a
		Def 函数b
			函数a
		在函数b中使用函数a
	5.8变量的作用域
		全局变量 在函数体内和函数体外都能发挥作用
		局部变量 定义在函数体中，只在函数内部发挥作用，函数运行完毕，变量销毁
		Global  关键字声明全局变量
6数据容器
	主要是为了批量储存数据
	列表 元组 字符串 集合 字典
	6.1 list
		1、列表定义
			变量名称=[]
			变量名称=list（）
		列表可以存储多个数据，可以为不同类型数，支持嵌套，列表嵌套列表，列表嵌套字典，集合等
		2、列表索引
			0元素1  1元素2  2元素2  3元素4  4元素5
			List[1],取出第二个元素
			最后一个-1 底数第二 -2
			嵌套列表list[1][0]
		3、列表常用操作
			列表提供的方法：插入 删除 清空 修改 统计
			方法：如果将函数定义为class的成员，则函数称为方法，只不过定义在class当中
			查找位置：List.index（）
			修改：list[索引] = 修改值
			插入：list.insert(下标，元素）
			追加：list.append（元素） #追加到结尾,单个元素
			追加：list.extend(元素)，追加多个元素到尾部
			删除：del list[下标]
			删除：list.pop（下标）
			##del是python的内置函数，关键字，list是一个类，pop就是类中的一个方法
			删除：list.remove(元素）
			统计：list.count(x)，统计列表中x的数量
			统计：len（列表），统计列表中元素数量
			清空：list.clear()
		4、列表的循环遍历
			While
			For
	6.2元组
		列表可以修改，元组不可被修改
		可以认为元组是一个只读的list
		定义：
			a=（元素1，元素2）
			a=tuple（元素1，元素2）
		操作方法：
			Index（），类内置方法
			Count（），类内置方法
			len（），关键字，自带函数
		循环遍历
			For while
		注意：元组的元素不能修改，但是元组内部的嵌套列表内容可以修改
	6.3字符串
		不可修改的数据容器
		可以直接生成新的字符串
		方法：
			索引String[]  Index  replace split strip()
			替换：string.replace(老字符串，新字符串)，不是修改是获得新字符串
			分割：string.replace(" 分割的符号") ,分割后得到列表
			规整：string.strip()，不传参数去除头尾空格
				例如 string = "12lsjfljslf21"
					strip（12）只要头尾有12，就去除，去除前后内容
		循环遍历
			While for
	6.4数据容器切片
		序列：内容连续、有序、可以使用下表索引的一类数据容器
		列表 元组 字符串都是
		切片操作：取出子序列
			语法：序列[起始下表:结束下标:步长]
			步长为1，一个一个取
			步长为2，跳过一个取，注意倒叙去，数字方向相反
	6.5集合
		集合最主要的特点是无序，不持支重复元素，可修改
		定义语法：
			a={，}
			a=set（）
		无序，不支持下标索引
		方法：
			添加：add，主动去重
			移除：remove（）
			取出：pop（）随机取，取出后，集合中该元素就不存在了
			清空：clear
			差集：set1.difference(set2)，去除集合1和集合2重合的部分，集合2不发生变法
			合并：set1.union(set2),集合1增加集合2中没有的元素，集合2不变
			统计：len
		遍历：
			while不能遍历，集合不支持下标索引
			for可以遍历
	6.6字典
			字典定义：
				a={key：value,key:value}
				a=dict()
			注意：字典key不可重复
			不可使用索引，可以通过key之索引，类型不限制，可以嵌套，把value作为一个内层字典即可
			字典嵌套可以实现查分
			方法：
				索引：dict["key"]
				索引：dict[key][key2]
				新增：dict【key】=value，key存在则更新值，key不存在，则新增
				删除：dict.pop（key）,找到key，并删除key和value
				清空：clear
				获取：dict.keys()获取全部key
				长度：len
				
				
			遍历：
				获取全部key进行遍历
				For key in keys:
					程序
				For key in my_dict:
				两种方法结果一直
				不支持下标索引，while循环不可用
	6.7比较
		通用支持
		Len min max 最大元素和最小元素
		字符串大小比较：
			大小写，数字，特殊字符，都有对应的ascll码表
			一位一位对比，只要第一个打，则字符串就大

7函数进阶
	7.1函数多返回值
		Return 1，3，返回1和3
		接受：x,y=tetst(），x接受1，y接收3
	7.2函数的传参方式
		位置参数：
			形参：1，2，3
			实参：a,b,c
			一一对应
		关键字参数：
			形参：name,age,gender
			传参：（name="",gender="",age=""）
			顺序不固定
		缺省参数：
			形参：（name,gender,age=20)
			后面不需要传参，已经有默认值
			后面也可以传参，则按照传递的去使用，默认参数必须在最后面
		不定长参数：
			参数数量不定：形参：*参数
			使用不定长传参时，会以元组的形式存储参数
			
			关键字传递：形参 ： **参数
			以字典形式储存，传入参数必须要有key和value，用key=value形式，例如，age=20
	7.3匿名函数
		1、函数作为参数传递：
			是计算逻辑的传递
			在函数体内部，被计算的数据是确定的，被计算的逻辑不确定，被计算的逻辑由谁决定？由传入的函数决定
			普通函数：逻辑确定，数据不确定
		2、lambda定义匿名函数
			语法：
				Lambda 传入参数 ： 函数体（一行代码）

8文件操作
	8.1文件编码
		翻译的规则，记录了如何将内容翻译成二进制，以及如何将二进制翻译回可识别的内容
	8.2文件读取操作
		1、打开文件
		open（name,mode,encoding), mode是权限 
		#注意，位置参数和关键字参数
		2、读写文件
			文件的方法：
			File.read(num) 指定读取多少字节
			多次调用read，下一次会从上一次读取过后的字节数开始读取
			File.readlines(),返回列表，每一行为一个元素
			File.readline()每次读取一行
			读取文件时候，都会有指针的影响，都会在上一次读取过后的结果进行操作，只要是操作文件内容，都存在指针
			循环读取行：
				For line in file：
		3、关闭文件
			File.close # 不关闭，文件就一直被占用，除非停止运行和close ，在python中文件应该也是一个类
		4、利用with open可以在操作结束后自动关闭close文件，避免遗忘掉close
			With open（） as f:
				f.readline
	8.3文件写出操作
		语法
			File.write("") #写入到内存中
			f.flush #把写入到内存中的文件写入到磁盘中
			f.close #close 内置了flush
	8.4文件追加操作
		W 写或创建，覆盖写
		A 最后追加写入，存在追加，不存在，创建
	
9异常处理
	9.1异常的捕获方法
		对异常进行提醒，整个程序继续运行
		语法：
			try：
				可能发生错误的代码
			except：
				如果异常执行的代码
		捕获指定异常：
			try：
				可能发生错误的代码
			Except Nameerror as e：#添加异常名称
				如果异常执行的代码
				print（e）
				可以将异常设置别名，打印出来
		捕获多个异常
			Except （error ，error）as e : #用元组储存多个异常名称
		
		捕获所有异常
			Except exception as e ： #捕获所有异常
			######学习的时候要先知道，这个东西是干什么的？目的是什么？为了解决什么问题？，这样就好学很多
			Try：有异常执行
			Else：没异常执行
			finally：有没有异常都要强制执行
	9.2异常的传递
		多个函数嵌套，在调用后面的函数时候，也可以捕捉到前面函数的异常
		主要是为了表明：并不需要深入的具体代码块去捕获异常，只需要在最顶级的调用中进行捕获即可
	9.3模块
		1、模块导入
			模块就是一个python文件，里面有类、函数、变量，可以导入后直接调用
			From 模块名 import 
			Import 模块名
			Import 模块1，模块2
			模块调用 modle.function()  模块名+函数/类()传入参数
			From time import sleep 从模块里面导入sleep这个方法
			可以直接使用sleep
			例如：
				sleep（5）
	9.4自定义模块并导入
		模块名就是文件名
			1、自定义模块my_modle1.py
			2、在该文件下定义一个函数fun_1
			3、导入，import my_modle1.py
			注意：函数-类-模块文件定义不要重名
		不想让模块中的测试代码执行，可以把测试代码放到__main__当中：
			If __name__ == '__main__':
				测试代码块
		注意：
			__all__  = ['test_a'] #模块文件
			调用时import *
			此时就是调用了整个__all__,其他非test_a的功能块是不能调用的
		
	9.5python包
		自定义python包
		python包太多，管理混乱，python包就是为了更好地管理模块
		python包就是一个文件夹，包含两类内容，一堆python模块和__init__.py的文件（初始化文件）
		1、导入包
			Import 包名.模块名
		2、自定义包，init__.py,不要忘记
		3、导入第三方包
			Pip install numpy
			Pip install -I url 包名 国内下载，快一点
		4、数据可视化图表：百度pyecharts
		
第二阶段

1对象
	1.1理解类
		 类，对象，属性
		设计表格（类）
		打印一张表格（给学生一个表格）（创建一个对象）
		填写表单（对属性进行赋值）
		#创建一个类：
			Class Student：#大写
				Name=none
				Gender=none  #定义这个类可以具有的属性，后面传入
				Def 函数：#定义这个类的方法，也就是这个类可以做什么？
		#创建一个对象
			Stu_1=Student（） #类似声明我这个对象属于这一类
		#对对象进行属性和方法赋值
			Stu_1.name="jack"
			Stu_1.gender="male"
			Stu_1.函数（）
	1.2类的方法
		Class Student：
			name = none
			age =none
			def say_hi(self):
				print(self.name) #在方法内访问成员变量必须使用self.varname，外部传入的参数不需要使用，可以直接引用
		类的方法定义：
			def方法名 （self,形参1，形参2）：
			必须要有self，作用就是为了表示类对象自身，传参的时候可以当作不存在
			在成员方法内部，要想方位类的成员变量，必须使用self
	1.3类和对象
		 面向对象就是让对象干活
		
	1.4构造方法
		问题：构建类对象的时候，能不能把成员变量的值给传递进去？
		传统构建类对象
			stu_1=Student（）
		能够变成
			stu_1 = Studeng(a,b)?
			这个括号，能够想函数，方法那样，通过传参的形式对属性赋值，注意，是对属性进行赋值，不是对方法进行赋值
		实现方式：构造方法
			_init__()：
			创建类对象的时候，会自动执行
			创建对象的时候，将传入的参数自动递归给__init__方法使用
		例如：
			def __init__:(self,name,age)：
				self.name=name
				self.age=age
			#创建对象并传入参数
			stu=Student("xiaoming",15)
			#调用属性
			stu.属性   #类名.属性
	1.5魔术方法
		这些方法可以帮助我们比较对象，尤其是对象具有某些属性的比较
		__str__ 可以把输出的类对象由内存地址转变成字符串
		__lt__可以把输出的类对象进行大小比较
		__le__用于小于等于和大于等于的比较
		__eq__判断类对象是否相等
	1.6封装
		面向对象三大特性，封装，继承，多态
		将属性和行为在类中描述为类中的变量和方法，就是封装
		私有成员属性和方法以两个下划线开头：
			__name=none
			def __test :
		注意：创建的对象私有属性和私有方法不能直接使用，但是私有属性和方法是为实现其他功能提供服务，是为了更好地实现功能，类的其他成员可以使用私有方法，也就是类内部的其他属性和方法可以调用私有属性和方法。
	1.7继承
		语法：
			class 类名（父类）： #单继承
				类内容
			class 类名（父类1，父类2，父类3）： #多继承
				类内容 / pass 补全语法，是空的不用写
			注意：多继承，同名成员属性和方法，左边继承的优先级更高
		复写父类：
			直接修改属性
			直接重新定义方法，就实现了重写父类属性和方法
		调用父类：（在子类中调用父类的属性和方法）
			方法1：父类名.变量
				 ：父类名.成员方法（self）
			方法2：super（）.成员变量
				：super（）.成员方法（）
	1.8类型注解
		语法：
			变量注解：var_1 : int =10
			类注解：
				class Student:
					pass
				sut: stu_1 = Student()
			容器类型注解和容器详细注解
			函数和方法的类型注解：
			形参类型注解：
				def add(x:int, y:int):
			返回值类型注解：def add(x:int, y:int)  ->list:
	1.9多态
		多种状态，完成某个行为时，使用不同对象，得到不同状态
		传入狗得到汪汪汪
		传入猫得到喵喵喵
		每个类都有同样的方法，但是方法对于不同类的对象表现不同
		多用于继承：class Animal：
				：class Dog(Animal)
					重写父类方法
				   class Cat（Animal）
					重写父类方法
		应用场景
			抽象类
			抽象方法
			例子：空调标准，不同厂家不同实现
抽象类多用于顶层设计，接口，是对子类的软性约束![image](https://github.com/taocheng18646/Document/assets/139728792/b7d03374-2410-4334-a608-74a09e71939a)
