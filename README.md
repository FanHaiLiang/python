# python 2016.11.28
# 什么是python
#### Python,是一种面向对象、解释性计算机程序语言，由Guido van Rossum于1989年发明，第一个公开发行版发行与1991年。python官网：https://www.python.org
# python能为我们做什么
#### web服务器编程，数据挖掘，自然语言处理，自动化测试等等
# python哲学
#### 优美、清晰、简单是python一直强调的哲学理念。
# python语言的特点
#### python语言的开放性赋予了其强大的生命，这与linux相同。
#### python是一门面向对象的语言，模块，变量，函数都看作是对象。
#### python有很好的跨平台性，也可以很容易和多种编程语言衔接，所以我们也称python为胶水语言。
#### python简单的特点，被用作学习的第一种编程语言很合适，性价比较高。
# python的核心数据类型
#### 数字(int/float),字符串(string)，列表(list)，字典(dict)，元祖(tuple)，集合(set)，文件。
#### 其他类型：类类型(object)None(Nonetype) 布尔型(Boolean)
#### 变成单元模块类型：函数(function)、模块(module)、类(class)
# python程序的组成
#### 程序由模块构成
#### 模块包含语句
#### 语句包含表达式
#### 表达式建立并处理对象
# 标识符命名规则
#### 1）标识符是由一个或多个字母、数字或下划线组成
#### 2) 标识符的第一个字符必须是字母或下划线
#### 2) 标识符不能与关键字相同
#### 4) python　是严格区分大小写的
# 标识符命名的默认规则
#### 1) 以单一双线开头的变量名(_x)　不会被from module inport *语句导入
#### 2) 前后双下划线的变量(__x__)　为系统的默认变量
#### 3)　前面两个下划线开头的变量(__x)为类的私有变量
# 变量的初始化和使用
#### 变量使用前必须赋值(初始化)
#### python属于弱类型变量：对象有类型变量无类型，变量就相当于一个对象的标签
#### python中变量和常量分开存放，当把变量重新赋值的时候即变量存放的地址发生了改变。不用的常量仍然在内存中，有自动的垃圾处理机制，如果没有变量绑定这个常量则自动会处理也可以通过del来处理，全局变量也随进程消亡。
# 两个数的交换
#### １) a,b = b,a 2) a ^= b,b ^= a,a ^= b (只对整数有效)　3) temp = a,a = b,b = temp
# 简单运算法则
#### / 取整除数　% 取余　（除数为小数商就有小数
## 位运算
#### 左移　a >> 2　表示在最右边加上两个零　相当于乘４
#### 右移　a << 2　表示删除最有边两位数　相当于除于４取整
#### a & b & 与　　两个数２进制进行比较　只要有一个数是1就取1
#### a | b | 或　　两个数２进制进行比较　只要有一个数是０就取０
#### a ^ b ^ 异或　两个数２进制进行比较　相同取０　不同取１
#### ~a 　　~ 取反　一个数的二进制数　取反　如：~14 １５
## 逻辑运算
#### == != or and not is:判断两个对象是否为同一个对象　isnot in notin 支持连逻辑运算：a>b>c +=等
# 运算符的优先级
#### yield x
# dir(math) 查看math（）包含的参数　dir　通用
# math模块
#### import math 引用math这个模块
#### math.sqrt(a) a开放
#### math.pow(a,b) a的b次方
#### math.trunc(a) 如果a是小数，省去小数部分　
#### math.floor(a) 对a向下求整，值小于或等于ａ
#### math.ceil(a) 对ａ向上求证，值大于或等于ａ
#### math.pi pi　常量等于3.1415926．．．．
#### math.e e=2.178281......
#### math.log(x[,base]) 对数运算(幂次方)，默认基地为e的对数运算。如：math.(8,2) 3.0
#### math.fabs(a) 对a取绝对值
#### math.factorial(a) 求a的阶乘
#### math.exp(a) 求e的a次方
# random模块
#### import random　引入random模块
#### random.random() 随机生成一组数
#### random.chice(数据类型)　在这个数据类型中随机挑选一个
#### random.randint(a,b) 生成随机数n　a <= n <= b
# 类型的强制转换
#### int(1.22) 将float转换成整型,省去小数部分 int('123') 将字符串转换成整型
#### str(123) 将整形转换成字符串等
#### repr(123) '123' 强转
#### ｀123｀ '123' 强转成字符串　　python３中没有反单引号这个强转
#### str(123) '123' 强转
# 字符串
#### 字符串：零个或多个字符组成的有限串行　必须用引号引起来，不区分单双引号　是一种容器数据类型，它是由多个字符组成的，不可变数据类型
#### len(a) : 显示字符串ａ的长度
#### a.count('l') 查看l的个数
#### a.repleace(a,l) 替换　将ａ编程ｌ
#### a.find('e') 查找第一个e的下标 找到返回索引值　找不到返回－１
#### a.index('a')　查看a的下标
#### a.upper() 将小写转化为大写的
#### a.split('　') 分割　以空格进行分割
#### s=' '.join(a) s ＝　等于以空格为拼接的a
#### a.isdigit() 判断a中是否都是数字
## 分片操作
#### 一般形式为x[i:j:z] 表示：取出在x中从索引值为i，直到但不包括索引值为j的内容，z表示步长　表示每z个去一个值
#### a='asdasd'a[1]: 's'
#### a[-1]: 'd'
#### a[1:3]: 'sd'
#### a[1:]: 'sdasd'
#### a[0:3]: 'asd'
#### a[:-1]: 'asdas'
#### a[:]: 'asdasd'
#### a[::-1] 'dsadsa' 逆向取值 每一个取一个
#### a[::-2] 'das' 　　逆向取值　每两个取一个
#### a[-1:-5:-2]  'da'
#### a[2::-2] 'da' 在２前边的每两个取一个
#### a = 'z' + a[1:] :表示把z代替第一个数
#### a = 'z' + a[2:] :表示把z代替前两个数
## 支持　＋　＊　进行合并/重复
#### a + 'xyz' 'asdasdxyz'
#### a * 2 'asdasdasdasd' 把整个字符串×２
# 输入
#### raw_input(): 无论输入什么类型　都当成字符串处理并返回　可以在前面直接加强转　如int(raw_input)
#### input(): 输入什么类型　输出什么类型
#### python3中没有了raw_input　只有input　作用和raw_input一样
# 输出
#### pirnt 在python2中　两个输出之间加都好不换行　不同字符串之间加逗号不换行
#### python3中　输出要用括号括起来　换行用end=""
# 格式化输出
格式化输出：
#### %d: 传入一个整形的　
#### ％s：传入字符串　
#### ％u: 不带符号的十进制
#### ％x:不带符号的１６进制
#### %X：不带符号的１６进制
#### %o:不带符号的８进制
#### ％e：科学计数法表示的浮点数
#### ％E：科学计数法表示的浮点数
#### ％f/F:十进制的浮点数
#### %g:如果指数大于－４或者小于精度值则和e相同，其他情况和f相同
#### %G:如果指数大于－４或者小于精度值则和e相同，其他情况和F相同
#### %c:单字节
#### $r:字符串
#### ％s:字符串
#### 如：print "the lenght is %s hello "%变量　print "the lenght is %s　％s hello "%(变量，变量)　传给两个数 打印一个％　用％％　输出一个％
# 修饰符
#### １．%字符：标记转换说明符的开始
#### ２．转换标志：－ 表示左对齐；＋表示在转换值之前要加上正负号；“”（空白字符）表示整数之前保留空格；０表示转换值若位数不够则用０填充
#### ３.最小字段值：转换后的字符串至少应该具有该值指定的宽度。如果×，则宽度会从值组中读出
#### ４.点（.）后跟精度值：如果转换的是实数，精度值就表示出现在小数点后的位数。如果转换的是字符串，那么该数字就表示最大字段宽度。print "this is %5.2f"%a 表示小数点后占两位　四舍五入
#### ５.字符串格式化转换类型
# 注释　＃
#### ‘’‘　文档的解释　’‘’　　多行注释的作用　不是多行注释　对文档解释作用
#### print math.__doc__　　查看模块的信息
# 列表
#### 列表：表示一种容器类型，有序的,可以是混合的　序列从０开始  是可变数据类型　支持切片操作　[]中括号是列表
#### l = [1,5，‘hello’,[4,8,6]] 　定义一个列表　
#### l[1] 5      l[3][1] 8
#### l[0] = 2 　　改变l中的第一个数
#### l.append('a') 向列表的末端加入a 　　　append : 附加
#### l.extend([5,6]) 合并两个列表　　　　　extend: 扩展
#### l.insert(3,2) 在下标为３的位置插入２　insert: 插入
#### l.index(5) 显示５的下标　１　　　　　　index: 指标　做索引　　　
#### l.count(2) 显示２的个数　　　　　　　　count: 数
#### l.sort() 排序　默认从小到大排序　　　　sort : 排序
#### l.pop()  显示最后一个元素　　　　　　　pop:　流行
#### l.reverse() 反转　　　　　　　　　　　reverse: 反转
#### del l[２] 删除下标为２的数　　　　　　　del:删除
#### len(l) 判断列表的长度
#### l.remoove(2) 删除值为２的数
# 元祖
#### 是一种容器类型，是任意对象的有序集合，通过索引访问　不可变类型　可以分片　()小括号是元祖
#### t = (1,2,3)  建一个元祖
#### 可以加法和乘法
#### 元祖只有一项是　加一个逗号
#### zip(t1,t) :形成一个元祖　如果t,t1都是　列表　那么生成生成一个大的列表其中包含几个元祖
# 序列
#### 序列：是指列表，字符串，元祖三个类型
#### 特点：１．可以通过索引来抓取特定的项目 ２．可以切片
#### max(x) :返回最大值 返回x中最大的值 min(x)：返回最小值 返回x中最小的值 '＊': 重复　str*5 　str　重复５次
#### cmp(x,y):比较２个序列值是否相等。字母的字符串长于数字的字符串１表示前面长于后面　－１表示后面长于前面　０表示相等
# 字典
#### 字典：通过键值对来实现元素的存取，是一种无序的集合，容器可变，可改变的　大括号｛｝没有运算 键：可以是数字或字符串，值什么类型都可以 内部查找是：散列查找 d = {‘a’:1,'b':2,'c':3} 
#### d.keys()   列出所有的键
#### d.values() 列出所有的值
#### d.items() 　列出所有的键和值　每一对形成一个元祖
#### d.get("a") 获取键a的值
#### d.update(d2)  合并
#### d.pop(key)     弹出某一个　字典中弹出的一个消失
#### del d[key]     删除 　用中括号
#### a = dict(zip(x,y)) 两个元祖x,y或者其他转换成字典
#### dict(zip(t1,t)) 生成字典
# bool:　只有两种　true false
# none 类型是　nonetye
# 集合
#### 集合　无序排列，可包含不同数据类型　支持成员关系测试　大括号{}　只能整体使用不可以取数　不可以有重复的项
####  s = {[1,2]} 定义一个集合
####  s = set([]) 定义一个空集合
####  s = {1,2} 定义一个集合
####  s=frozenset({1,2,3}) frozenser定义的列表不可变　　　frozen:　冰冻
####  s.add(5)　　　　　　　添加一个值
####  s.pop() 　　　　　　　随机弹出
####  s.clear()    　　　　清空集合
####  s.remove(1)   　　　 删除集合中某个数
####  s.diffreence(s1) 　　 列出s中有s1没有的项
####  s.union(s1)  　　　　 合并s和s1中　相同的只取一项
####  s.update(s1)  　　　　合并s和s1　　相同的只取一项
##  集合的运算
####  s - s1     　　　　　　减去s1中和s中重复的项
####  s | s1     　　　　　　合并(并集)
####  s & s1    　　　　　　 相同的（交集）
####  s ^ s1    　　　　　 　不相同的（补集
# 数据类型总结：
####    bool : 　　 true  false 　逻辑运算得到的结果为bool类型
####    nonetype:　  none 　用作空，占位变量
####    数字  　整型/浮点型　　  不可变的　 数学运算位运算等
####    字符串　　   　有序的　  不可变的　＋*运算　　属性方法　切片操作　 in逻辑
####    列表　　　　　　有序的　  可变的　　＋*运算　　属性方法　切片操作　 in逻辑
####    元祖　　　　　　有序的　  不可变的　＋*运算　　属性方法　切片操作　 in逻辑
####    字典          无序的　  可变的　　　　　　　　属性方法　　　　　　in逻辑（键）
####    集合   set{}  无序的　  可变的　  －｜^&运算　 属性方法　　　　　　in逻辑
####       frozenset 无序的　  不可变　  －｜^&运算　 属性方法　　　　　　in逻辑
# copy
#### 1. copy.copy 浅拷贝 只拷贝父对象，不会拷贝对象的内部的子对象。
#### 2. copy.deepcopy 深拷贝 拷贝对象及其子对象
# if语句 
if 判断条件:
     语句块/pass　pass:占位符　什么都不执行
if 判断条件：
     语句块　
else:(如果if条件不成立时执行这个)
     语句块
if 判断条件１:
     语句块
elif 判断条件２:(当判断条件１不成立时执行这个 可以嵌套无数个这个)
     语句块
else:(当判断条件１/２都不成立时　执行这个)语句块
## 三元运算：x if 判断条件 else z 如果判断条件是真的返回x,如果判断条件是假返回z
# range
#### range　快速生成一个序列
#### range（i,j,[步进值]）：i:起始值　j：终止值但不包括　
#### range(10) 生成一个0到10的序列
#### srange(10):形成一个迭代对象
# for循环
for 变量　in　列表:
     语句块
for 变量　in　列表:
     语句块
else:
     语句块
#### 列表　可以使字符串　元祖　序列　表达式　等
#### 同时满足多个变量的赋值　前面几项后面必须几项 如 for (i,j) in [(1,2),(1,2),(1,2)]: print i,j
## for循环3元表达式
 [x for x in [1,2,3]]  生成[1,2,3]
 [x+1 for x in [1,2,3]] 生成[2,3,4]
 [x+y for x,y in [(1,2),(3,4)]] [3,7]
 [x for x in range(101) if not x % 2]
# "迭代指重复执行一个命令"
# 获取索引和值的方法
#### for i in range(len('hello')): print i
#### 获取序列中的值的方法 遍历 for i in "hello": print i
# while循环
while 判断语句:
     语句块
while 判断语句:
     语句块
else:
     语句块
# 循环控制
#### break:　　　循环直接结束，下面循环不执行　　　　　　　　 　
#### continue:  跳出本次循环　执行下次判断　再循环
# 控制语句总结：
#### 顺序执行，选择分支，循环
#### 分支语句　
####     if elif else
####     简单的if语句
####     if...else
####     if...elif....else
####      f 的嵌套
####      x if y else z
###       循环　
####      while...else   while True:死循环 循环结束条件 与break continue配合
####  for  ...else 多种形式的集合类型 与range的配合 多个变量接收 [x for x in range(100)]
#### break:　　　结束循环
#### continue:　跳出本次循环
#### pass:　　　　空占位符
# 函数
#### 函数是一个完成特定功能的代码模块，其程序代码独立，通常有返回值，也可以是空值。最小的封装单元
## 为什么用函数：
#### １.可以重复使用　　2.增加封装特性　１）代码保密　２）规定使用方法　３）无需了解实现机制　４）使代码美观
## 內建函数：
#### 系统定义好的　dir(__builtin__) 查看内建函数
## 方法
#### 在一个类中的函数叫方法
## API(接口)
#### 是一些预先定义的函数，目的是提供应用程序与开发人员基于某软件或硬件得以访问一组例程的能力，而又无需访问源码，或理解内部工作机制的细节
## 函数三要素：
#### １.功能: 确定函数的功能是设计一个函数的前提。所谓功能就是函数最终要实现什么，决定了一个函数的复杂程度，运用什么方法，还是呢么样的逻辑设计　
#### ２．参数 :也叫参变量，是一个变量。也成为形参，通常在函数没有被调用时候形参
#### ３．返回值：返回值是函数执行结束后调用形式返回给调用者的结果。如果一个单纯的功能函数那么也可以没有返回值。没有返回值默认返回none　如果有返回值则用return标识
## 函数的定义
del 函数名(参数值(可以加也可以不加)):　
    语句块（函数内部的功能)
    return 可以多个返回值　函数执行到return的时候　函数立刻结束　后面的不会执行了
例：　　　
def fun1(a,b):
  return a+b,a-b
print fun1(3,2) 输出(5,1) 以元祖的形式传出
## 传参
### 共享引用
#### 1. 函数的形参变量只是在函数内起作用，这种参数的传递实际上是一种引用的共享，即把本地对象与形参变量相联系。
#### 2. 对于不可变变量，当在函数内改变变量值时候只是让这个形参指向了一个新的对象。所以这种改变不会影响原来的本地变量的值。
#### 3. 对于可变变量，如果在函数内修改了值，那么会对原来的引用产生影响。即原来变量的值也会发生改变。这样的做法是Python的一种机制。
### 避免可变参数的修改
#### 1.直接传递可变对象的副本 a = a[:]
#### 2.转化为不可变对象
#### １．定义位置参数的函数
def fun(a,b):
    print a,b
fun(1,2)
#### ２．定义默认值传参 允许什么都不传　打印默认值　传入一个数　输入传出的数 默认值参数必须放在后面
def fun1(a,b = 100,c=1000):　
    print a,b,c
    fun1(1,2)
#### ３．*传参  收集位置参数　　可以传入任意数目的参数
def fun2(*a):        fu2(a,*b) 把第一个传给a 剩下的传给b
    print a
    fun2(1,2,3,4,5,6)
#### ４．**传参　收集字典的方式
def fun3(**a)   　　　必须这个顺序a,d=100,*a,**a
    pringt a
    fun3(a = 1,b=2)
#### 在python3中可以这样 2中不行
def fun4(*a,b):
    print （a,b）
    run4(1,2,3,b=100)
#### 传参过程中：
def fun(a,b):
    print a,b
#### 1.位置传参
fun(1,2)
#### 2.关键字传参
fun(b = 1,a = 2) 要求名字和关键字名一样
#### 3.*传参
l = [5,6]
fun(*l)
#### 4**传参
d = {"a":1,"b":2}  ＝＝＝＝》a = 1,b = 2
fun(**d)
