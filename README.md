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
#### pirnt 在python2中　两个输出之间加都好不换行　不同字符串之间加都好
