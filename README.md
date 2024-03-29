# python_1
第一天
解释器
	计算机不能直接理解任何除机器语言以外的语言，所有必须要把程序员所写的程序语言翻译成机器语言，计算机才能执行程序。将其他语言翻译成机器语言的工具，称为编译器。
编译器翻译的方式
	1.编译
	2.解释
	区别在于翻译时间点的不同，当编译器以解释方式运行的时候，也称之为编译器。
	编译型语言：程序在执行之前需要一个专门的编译过程，把程序编译成为机器语言的文件。运行时不需要重新翻译，直接使用编译的结果就行了。程序执行效率高，依赖编译器，跨平台性差些。如c，c++语言。
	解释型语言：解释型语言编写的程序不进行预先编译，以文本方式储存代码，会将代码一句一句直接运行。在发布程序的时候，看起来省了到编译工序。但是在运行程序的时候，必须先解释再运行。
	
python的设计目标
	1. 一门简单直观的语言并与主要竞争者一样强大。
	2. 开源，以便任何人都可以为他做贡献。
	3. 代码像纯英语那样容易理解。
	4. 适用于短期开发的日常任务。
python开发者的哲学
	用一种方法，最好是最有一种方法来做一件事。如果面临多种选择，python开发者一般会拒绝花俏的语法，而选择明确没有或者很少有歧义的语法。
python特点

是完全面向对象的语言
	1.函数，模块，数字，字符串都是对象，在python中一切皆为对象。
	2.完全支持继承，重载，多重继承。
	3.支持重载运算符，也支持泛型设计。
python用有一个强大的标准的数据库
	python语言的核心只包含数字，字符串，列表，字典，文件等常见类型和函数。而由python标准库提供了系统管理，网络通信，文本处理，数据库接口，图形系统，XML处理等额外的功能。
python社区
	提供了大量的第三方模块，使用方式与标准库类似。它们的功能覆盖科学计算，人工智能，机器学习，web开发，数据库接口，图形系统多个领域。

python优点
	1.简单，易学。
	2.免费，开源。
	3.面向对象。
	4.丰富的库。
	5.可扩展性。
		如果需要一段关键代码运行的更快或者希望某些算法不公开，可以把这部分程序用c或c++编写，然后在python程序中使用它们。
python缺点
	1.运行速度。
	2.国内市场较小。
	3.中文资料匮乏。

python源程序的基本概念
	python源程序就是一个特殊格式的文本文件，可以使用任意文本编辑软件做python的开发。
	python程序的文件扩展名通常都是  .py  。

print（“内容”）  ：输出内容。    不要加分号。

交互式运行python程序
   直接在终端中运行解释器，而不输入要执行的文件名
	在终端中输入 $ python3     如果前面自带$则不用加$.
	然后会出现3个箭头，在箭头后面输入代码。
	 优点
		适合学习，验证python语法或局部代码。
	 缺点
		代码不能保存。
		不适合运行太大的程序。
退出官方的编辑器
	1.直接输入exit（）。
	2.使用热键退出  ctrl+d。

pycharm介绍
	1.它是python的一款非常优秀的集成开发环境。
	2.除了具有一般IDE所具备的功能外，还可以在linux，windows，macOS中使用。
	3.适用于大型开发项目。
		一个项目中通常会包含多个源文件。
		每个源文件的代码行是有限的，通常在几百行之内。
		每个源文件各司其职，共同完成复杂的业务功能。
Python 命名规则
	文件名不可以用数字开头。
	命名文件名的时候建议只用小写字母，数字，下划线。 
	
python注释
	单行注释： # 说明文字。
		为了方便他人查看，注意注释和代码之间最少要有两个空格。
	多行注释： ”“”   内容     “”“      
		被3个双引号中括中的内容都是注释。

python算术运算符
     +  ：加  3+2=5。
	-  :   减  3-2=1。
    *   ：乘  1*2=2。 
    /   ：除   2/1=2。
    //  ：取整除    9//2=4。
    %   ：取余数   9%2=1。
    **   ：幂     2**3=8。
*      还可以用于字符串，计算结果就是字符串重复指定次数的结果。
例如 
	“-”*3=‘---’  。

变量
	程序是用来处理数据的，变量是用来存储数据的。
  在python中，每个变量在使用前都必须要赋值，变量赋值以后该变量才会被创建。
  等号（=）用来给变量赋值。
	变量名=值
		变量定义后就可以直接使用。
	例如
		a=“123456”
		print（a）
			不需要分号和双引号。
	变量名只有第一次出现的时候才是定义变量。
	变量名再次出现，不是定义变量，而是使用之前定义过的变量。
	
  在python中，定义变量时是不需要指定变量类型的。
  在运行的时候，python解释器，会根据赋值语句等号右侧的数据自动推导出变量中保存数据的准确类型。
	Int ：整数类型
	Str ：字符串类型
	bool：布尔类型  （真或假）（true或false）  true=1  false=0。
	float：浮点数（小数）类型
	complex： 复数型
		主要应用于科学计算。
非数字型
	字符串
	列表
	元组
	字典
python中，字符串直接可以使用+拼接成新的字符串。
	例如
		a=啊
		b=啊
		c=a+b
		print（c）
		
	会显示出啊啊

变量的输入
	在python中需要使用input函数
	使用input函数后，用户输入的任何内容python都会认为是一个字符串。
	语法
	input（“请输入内容”）
		会显示出     请输入内容
	a=input（“请输入内容”）
		则会把用户输入的内容赋给a。
	
类型转换函数
	int（x）  ：  把x转换为整数。
	float（x） :   把x转化为浮点数。
	具体使用
		int（input（“请输入一个数”））  ：将字符串变为整型
		a=input（“请输入一个数”）
		a=int（a）  ：将a变为整型
	
变量的格式化输出
	% ：格式化操作符
		%s  ： 字符串
		%d ： 有符号10进制整数，%06d 表示输出的整数显示位数，不足的地方用0补齐。
		%f  ： 浮点数，%.02f 表示小数点后只显示2位
		%% ：输出%
	格式
		print（“%s”%n）  
		print（“格式化字符串”%（变量1，变量2……））
		
变量的命名
	标识符和关键字
		
		标识符
			标识符就是程序员定义的变量名，函数名。
			标识符可以由字母，数字，下划线构成。但是不能以数字开头，不可以与关键字重名。
		关键字
			python内部已经使用的标识符。
			关键字具有特殊的功能和含义。
			开发者不允许定义和关键字相同的名字的标识符。
				import 关键字 可以导入一个“工具包”
				在python中不同的工具包，提供有不同的工具。
		变量的命名规则
			python中的标识符是区分大小写。
			在定义变量的时候，为了保证代码格式，= 的左右应该各保留一个空格。
			在python中，如果变量名需要两个或者多个单词构成时，可以按照以下方式来命名
				1.每个单词都使用小写字母。
				2.单词与单词之间用下划线连接。
					例如 ： first_name 
				也可以使用驼峰命名法
					小驼峰命名法：第一个单词用小写，后续单词首字母用大写。
						例如： firstName
					大驼峰命名法 ：每一个单词的首字母都采用大写
						例如： FirstName
判断（if）
	if 要判断的条件：
		条件成立的后要做的事情。
												代码的缩进为一个tab或者4个空格。
												在python开发中不要将空格和tab混用。
	else：
		条件不成立时，要做的事情。

算术运算符
	== ：检查两个操作数是否相等。若相等返回true
	！= ：检查两个操作数的值是否不相等。若不相等返回true
         > :  大于。
           <  :  小于。
         >=  : 大于等于。
         <= : 小于等于。
   在python 2.x中 <>可以代表不等于。

逻辑运算
	逻辑运算符
		and : 与
		or ：或者
		not ：非
elif
	跟c语言中else if 是一个道理。
	elif和else都必须配合if使用。
		elif 条件：
			条件成立时，执行的代码。
if（(a > 2 and b>2) or (c > 2 and d > 2) or (e > 2 and f > 2)）
	跟
if ((a > 2 and b > 2)                   缩进
		or (c > 2 and d > 2)   应该空两个tab键或者8个空格。
		or (e > 2 and f > 2))     为了让下面的 if 更好的识别所有空2个tab或8个空格。
	一样

如何在python中使用随机数
	Import random    导入随机数的模块 ‘工具包’
	Ipython 中 可以直接在模块后面敲一个 . 然后按tab键，会提示该模块中包含的所有函数。
	random.randint（a，b）返回a，b范围内的整数，包含a，b
	A = random.randint（a，b）  A直接为整数，不是字符。  为int型
	
while循环
	While 判断条件：
		条件满足的时，做的事情
		条件改变

赋值运算符
	= ：赋值
	+= ：加法赋值  例：c+=a 就是 c = c+a
	-= ： 减法赋值  例：c-=a  就是 c = c-a
	*= ：乘法赋值  例 ： c *= a 就是 c=c*a
	/= ：除法赋值 例 ： c /= a  就是 c=c/a
	//= ：取整除法赋值 例 ：c //= a 就是 c = c // a
	%= ：取余除法赋值 例 : c %=a 就是 c = c % a
	**= ：幂赋值   例 ： c **= a 就是 c = c**a

转义符
	\\ :反斜杠符号
	\' :单引号
	\"  :双引号
	\n :换行
	\t  :横向制表符
	\r :回车
	
函数的定义
	def 函数名（）：
		函数封装的代码
		。。。。。
		
	函数名称应该能够表达函数封装代码的功能，方便后续的调用。
	函数名称的命名应该符合标识符的命名规则。
		可以由数字，下划线，字母组成。
		不可以由数字开头。
		不可以和关键字重名。
	函数定义后，如果不调用函数，是无法执行的。
函数调用
	通过函数名（） 即可完成对函数的调用
	函数调用不可以在定义函数上方

pycharm的调试工具
	F8 step over 可以单步执行代码，会把函数当作一行代码执行。
	F7 step into 可以单步执行代码，如果是函数，会进入函数内部。
	
函数的注释
	要不然在函数名上2行后注释，但是很不方便，不推荐使用。
	在函数名下一行注释，并且可以使用 python中  view     quick documentation 方便查看函数注释
		快捷键  ctrl+q

函数的参数
	def 函数名（参数）：
	
函数的返回值
	返回值是函数完成工作后，最后给调用者的一个结果。
	在函数中使用return关键字可以返回结果。
	调用函数一方，可以使用变量来接受函数的返回结果。
		用return表示返回，后续的代码都不会执行。
		
形参和实参
	形参：定义函数时，小括号中的参数，是用来接受参数用的，在函数内部作为变量使用。
	实参：调用函数时，小括号中的参数，是用来把数据传递到函数内部用的。
	
函数的返回值
	返回值是函数完成工作后，最后给调用者的一个结果。
	在函数中使用return 返回结果。

	
函数的嵌套调用
	一个函数里面又调用了另一个函数，这就是函数嵌套调用。
	
使用模块中的函数
	模块是python程序架构的一个核心概念
		模块好比是工具包，要想使用这个工具包中的工具，就需要导入import这个模块。
		每一个以扩展名py结尾的python的源代码文件都是一个模块。
		在模块中定义的全局变量，函数都是模块能够提供给外界直接使用的工具。
	导入后，可以使用 模块名.变量/模块名.函数 的方式，使用这个模块中定义的变量或者函数。
	好处：模块可以让曾经编写过的代码反复使用。
	模块名是一个标识符（不能用数字开头）
		只能用数字，字母，下划线。
	
pyc文件
	python解释器为了提高性能，会把import导入的模块先编译成一个二进制文件（字节码）。python在执行文件的速度就有了非常明显的改善。
	
python中数据类型
	数字型和非数字型
		数字型：int 整型，float 浮点型，bool 布尔型，complex 复数型。
		非数字型：字符串，列表，元组，字典。
			在python中，所有非数字型变量都支持
				1.都是一个序列，也可以理解为容器。
				2.取值 【】。
				3.遍历 for in 。
				4.计算长度，最大/最小值，比较，删除。
				5.链接 + 和重复 * 。
				6.切片。
				
列表
	列表是python中使用最频繁的数据类型，在其他语言中通常叫做数组。
		专门用于存储一串信息。
		列表用【】定义，数据之间用 ，分割。
		列表的索引从0开始。
			索引就是数据在列表中的位置编号，索引又可以被称为下表。
			    a=[1,2,3]
			     a[0]=1
	查找：
		列表名.index（内容）
			可以查看内容对应数组的索引。
	修改：
		列表名[需要修改的索引]=修改内容
	增加：
		列表名.append（增加内容）   向列表末尾追加数据。
		列表名.insert（需要插入内容的索引，内容）   向某个区域增加内容
		列表名1.extend（数组名2）  向列表名1的末尾增加列表名2中的全部内容
	删除：
		列表名.remove（需要删除的内容）    删除列表中某个内容
		列表名.pop()     删除列表中最后一个内容。
		列表名.pop（需要删除内容的索引）   删除某个区域内容
		列表名.clear（）  清空列表
		del 列表名【需要删除的索引】
		del 列表名   删除该列表
			del删除是从将一个变量内存上删除的，后续就无法使用该列表。
	统计：
		len（列表名）  统计并且输出列表名中元素的个数。
			S = len（列表名）   将元素的个数给S。
		列表名.count（需要统计的数据） 统计列表中某一个数据出现的次数。
			S=列表名.count（需要统计的数据）  将某一个数据出现的次数给S。
	排序：
		升序：列表名.sort（）
		降序：列表名.sort（reverse=Ture）
		逆序：列表名.reverse（）
	循环遍历：
		遍历就是从头到尾依次从列表中获取数据。
			在循环体内部针对每一个元素，执行相同的操作。
		for 变量名 in 需要遍历的变量：
			运行内容
		
					例如
						name_list=【“张三”，“李四”】
						for my_name in name_list：
							print（“我的名字是%s”% my_name）
					运行结果为
						我的名字是张三
						我的名字是李四

元组
	 tuple 元组与列表类似，不同之处在于元组中的元素是无法修改的。
		元组表示多个元素组成的序列。
		元组在python开发中，有特定的应用场景。
			1.用于储存一串信息，数据之间使用 ，分隔
			2.元组用（）定义
			3.元组的索引从0开始
				索引就是数据在元组中的位置编号。
	定义元组
		元组名=（）     定义了一个空元组
		如何定义一个元组中只包含一个元素的元组
			元组名=（元素，）
				该元组中只包含了一个元素。
		
		
				
		 
