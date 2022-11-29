注：只学习机器学习需用用到的知识，其他不学。

位运算符
操作符	名称	实例
~	按位取反	~4
&	按位与	4 & 5
`	`	按位或
^	按位异或	4 ^ 5
<<	左移	4 << 2
>>	右移	4 >> 2
算数运算符
算数运算符是 运算符的一种
是完成基本的算术运算使用的符号，用来处理四则运算
运算符	描述	实例
+	加	
-	减	
*	乘	
/	除	
//	取整除	返回除法的整数部分（商） 9 // 2 输出结果 4
%	取余数	返回除法的余数 9 % 2 = 1
**	幂	又称次方、乘方，2 ** 3 = 8
在 Python 中 * 运算符还可以用于字符串，计算结果就是字符串重复指定次数的结果
In [1]: "-" * 50
Out[1]: '----------------------------------------' 
input 函数实现键盘输入
字符串变量 = input("提示信息：")
变量的格式化输出
格式化字符	含义
%s	字符串
%d	有符号十进制整数，%06d 表示输出的整数显示位数，不足的地方使用 0 补全
%f	浮点数，%.2f 表示小数点后只显示两位
%%	输出 %
语法格式如下：
print("格式化字符串" % 变量1)

print("格式化字符串" % (变量1, 变量2...))
print("我的名字叫 %s，请多多关照！" % name)
print("我的学号是 %06d" % student_no)
print("苹果单价 %.02f 元／斤，购买 %.02f 斤，需要支付 %.02f 元" % (price, weight, money))
print("数据比例是 %.02f%%" % (scale * 100))
随机数的处理
import random
random.randint(12, 20)  # 生成的随机数n: 12 <= n <= 20   
random.randint(20, 20)  # 结果永远是 20   
random.randint(20, 10)  # 该语句是错误的，下限必须小于上限
字符串中的转义字符
\t 在控制台输出一个 制表符，协助在输出文本时 垂直方向 保持对齐
\n 在控制台输出一个 换行符
列表常用操作
在 ipython3 中定义一个 列表，例如：name_list = []
序号	分类	关键字 / 函数 / 方法	说明
1	增加	列表.insert(索引, 数据)	在指定位置插入数据| | | 列表.append(数据) | 在末尾追加数据
列表.extend(列表2)	将列表2 的数据追加到列表
2	修改	列表[索引] = 数据	修改指定索引的数据
3	删除	del 列表[索引]	删除指定索引的数据
列表.remove[数据]	删除第一个出现的指定数据
列表.pop	删除末尾数据
列表.pop(索引)	删除指定索引数据
列表.clear	清空列表
4	统计	len(列表)	列表长度
列表.count(数据)	数据在列表中出现的次数
5	排序	列表.sort()	升序排序
列表.sort(reverse=True)	降序排序
列表.reverse()	逆序、反转
del 关键字（科普）
使用 del 关键字(delete) 同样可以删除列表中元素
del 关键字本质上是用来 将一个变量从内存中删除的
如果使用 del 关键字将变量从内存中删除，后续的代码就不能再使用这个变量了
del name_list[1]
元组
Tuple（元组）与列表类似，不同之处在于元组的 元素不能修改
元组 表示多个元素组成的序列
元组 在 Python 开发中，有特定的应用场景
用于存储 一串 信息，数据 之间使用 , 分隔
元组用 () 定义
元组的 索引 从 0 开始
索引 就是数据在 元组 中的位置编号
info_tuple = ("zhangsan", 18, 1.75)
元组中 只包含一个元素 时，需要 在元素后面添加逗号
info_tuple = (50, )
元组和列表之间的转换
使用 list 函数可以把元组转换成列表
list(元组) 
使用 tuple 函数可以把列表转换成元组
tuple(列表)
4.2 字符串的常用操作
在 ipython3 中定义一个 字符串，例如：hello_str = ""
输入 hello_str. 按下 TAB 键，ipython 会提示 字符串 能够使用的 **方法
1) 判断类型 - 9
方法	说明
string.isspace()	如果 string 中只包含空格，则返回 True
string.isalnum()	如果 string 至少有一个字符并且所有字符都是字母或数字则返回 True
string.isalpha()	如果 string 至少有一个字符并且所有字符都是字母则返回 True
string.isdecimal()	如果 string 只包含数字则返回 True，全角数字
string.isdigit()	如果 string 只包含数字则返回 True，全角数字、⑴、\u00b2
string.isnumeric()	如果 string 只包含数字则返回 True，全角数字，汉字数字
string.istitle()	如果 string 是标题化的(每个单词的首字母大写)则返回 True
string.islower()	如果 string 中包含至少一个区分大小写的字符，并且所有这些(区分大小写的)字符都是小写，则返回 True
string.isupper()	如果 string 中包含至少一个区分大小写的字符，并且所有这些(区分大小写的)字符都是大写，则返回 True
2) 查找和替换 - 7
方法	说明
string.startswith(str)	检查字符串是否是以 str 开头，是则返回 True
string.endswith(str)	检查字符串是否是以 str 结束，是则返回 True
string.find(str, start=0, end=len(string))	检测 str 是否包含在 string 中，如果 start 和 end 指定范围，则检查是否包含在指定范围内，如果是返回开始的索引值，否则返回 -1
string.rfind(str, start=0, end=len(string))	类似于 find()，不过是从右边开始查找
string.index(str, start=0, end=len(string))	跟 find() 方法类似，不过如果 str 不在 string 会报错
string.rindex(str, start=0, end=len(string))	类似于 index()，不过是从右边开始
string.replace(old_str, new_str, num=string.count(old))	把 string 中的 old_str 替换成 new_str，如果 num 指定，则替换不超过 num 次
3) 大小写转换 - 5
方法	说明
string.capitalize()	把字符串的第一个字符大写
string.title()	把字符串的每个单词首字母大写
string.lower()	转换 string 中所有大写字符为小写
string.upper()	转换 string 中的小写字母为大写
string.swapcase()	翻转 string 中的大小写
4) 文本对齐 - 3
方法	说明
string.ljust(width)	返回一个原字符串左对齐，并使用空格填充至长度 width 的新字符串
string.rjust(width)	返回一个原字符串右对齐，并使用空格填充至长度 width 的新字符串
string.center(width)	返回一个原字符串居中，并使用空格填充至长度 width 的新字符串
5) 去除空白字符 - 3
方法	说明
string.lstrip()	截掉 string 左边（开始）的空白字符
string.rstrip()	截掉 string 右边（末尾）的空白字符
string.strip()	截掉 string 左右两边的空白字符
6) 拆分和连接 - 5
方法	说明
string.partition(str)	把字符串 string 分成一个 3 元素的元组 (str前面, str, str后面)
string.rpartition(str)	类似于 partition() 方法，不过是从右边开始查找
string.split(str=“”, num)	以 str 为分隔符拆分 string，如果 num 有指定值，则仅分隔 num + 1 个子字符串，str 默认包含 ‘\r’, ‘\t’, ‘\n’ 和空格
string.splitlines()	按照行(‘\r’, ‘\n’, ‘\r\n’)分隔，返回一个包含各行作为元素的列表
string.join(seq)	以 string 作为分隔符，将 seq 中所有的元素（的字符串表示）合并为一个新的字符串
4.3 字符串的切片
切片 方法适用于 字符串、列表、元组

切片 使用 索引值 来限定范围，从一个大的 字符串 中 切出 小的 字符串
列表 和 元组 都是 有序 的集合，都能够 通过索引值 获取到对应的数据
字典 是一个 无序 的集合，是使用 键值对 保存数据
演练需求
截取从 2 ~ 5 位置 的字符串
截取从 2 ~ 末尾 的字符串
截取从 开始 ~ 5 位置 的字符串
截取完整的字符串
从开始位置，每隔一个字符截取字符串
从索引 1 开始，每隔一个取一个
截取从 2 ~ 末尾 - 1 的字符串
截取字符串末尾两个字符
字符串的逆序（面试题）
答案

num_str = "0123456789"

# 1. 截取从 2 ~ 5 位置 的字符串
print(num_str[2:6])

# 2. 截取从 2 ~ `末尾` 的字符串
print(num_str[2:])

# 3. 截取从 `开始` ~ 5 位置 的字符串
print(num_str[:6])

# 4. 截取完整的字符串
print(num_str[:])

# 5. 从开始位置，每隔一个字符截取字符串
print(num_str[::2])

# 6. 从索引 1 开始，每隔一个取一个
print(num_str[1::2])

# 倒序切片
# -1 表示倒数第一个字符
print(num_str[-1])

# 7. 截取从 2 ~ `末尾 - 1` 的字符串
print(num_str[2:-1])

# 8. 截取字符串末尾两个字符
print(num_str[-2:])

# 9. 字符串的逆序（面试题）
print(num_str[::-1])
enumerate()函数
enumerate(sequence, [start=0])
sequence：一个序列、迭代器或其他支持迭代对象。
start：下标起始位置。
返回 enumerate(枚举) 对象

seasons = ['Spring', 'Summer', 'Fall', 'Winter']
lst = list(enumerate(seasons))
print(lst)
# [(0, 'Spring'), (1, 'Summer'), (2, 'Fall'), (3, 'Winter')]
lst = list(enumerate(seasons, start=1))  # 下标从 1 开始
print(lst)
# [(1, 'Spring'), (2, 'Summer'), (3, 'Fall'), (4, 'Winter')]
enumerate()与 for 循环的结合使用。

for i, a in enumerate(A)
    do something with a  
公共方法

5.1 Python 内置函数
Python 包含了以下内置函数：

函数	描述	备注
len(item)	计算容器中元素个数	
del(item)	删除变量	del 有两种方式
max(item)	返回容器中元素最大值	如果是字典，只针对 key 比较
min(item)	返回容器中元素最小值	如果是字典，只针对 key 比较
cmp(item1, item2)	比较两个值，-1 小于/0 相等/1 大于	Python 3.x 取消了 cmp 函数
注意

字符串 比较符合以下规则： “0” < “A” < “a”
切片
| 描述 | Python 表达式 | 结果 | 支持的数据类型 |
| :—: | — | — | — | — |
| 切片 | “0123456789”[::-2] | “97531” | 字符串、列表、元组 |

切片 使用 索引值 来限定范围，从一个大的 字符串 中 切出 小的 字符串
列表 和 元组 都是 有序 的集合，都能够 通过索引值 获取到对应的数据
字典 是一个 无序 的集合，是使用 键值对 保存数据
异常
一个try语句可能包含多个except子句，分别来处理不同的特定的异常。最多只有一个分支会被执行。
try:
    int("abc")
    s = 1 + '1'
    f = open('test.txt')
    print(f.read())
    f.close()
except OSError as error:
    print('打开文件出错\n原因是：' + str(error))
except TypeError as error:
    print('类型出错\n原因是：' + str(error))
except ValueError as error:
    print('数值出错\n原因是：' + str(error))

# 数值出错
# 原因是：invalid literal for int() with base 10: 'abc'


try - except - finally 语句
不管try子句里面有没有发生异常，finally子句都会执行。
try - except - else 语句
子句执行时没有发生异常，Python将执行else

try:
    int("abc")
    s = 1 + '1'
    f = open('test.txt')
    print(f.read())
    f.close()
except OSError as error:
    print('打开文件出错\n原因是：' + str(error))
else:
# 没有报异常就执行这一步
raise语句
python通过 raise NameError(‘HiThere’) 抛出指定名称异常

try:
    raise NameError('HiThere')
except NameError:
    print('An exception flew by!')
    
# An exception flew by!
