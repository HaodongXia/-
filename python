Python学习笔记

在Python中所有非数字型变量都支持以下特点：

都可以是一个序列或容器，取值[], 遍历for in, 计算长度，最大最小值，比较，删除，链接+，重复*，切片

2、列表List

- 用于存储一串信息

- 用[]定义，数据之间用，隔开

- 索引从0开始

常用操作：

1. sort（）升序排序

2. append  

   name_list = ['Tom', 'Lily', 'Rose']

   name_list.append('xiaoming')

   \# 结果：['Tom', 'Lily', 'Rose', 'xiaoming']

   print(name_list)

3. clear

   name_list = ['Tom', 'Lily', 'Rose']

   name_list.clear()

   print(name_list) # 结果： []

4. insert

   name_list = ['Tom', 'Lily', 'Rose']

   name_list.insert(1, 'xiaoming')

   \# 结果：['Tom', 'xiaoming', 'Lily', 'Rose']

   print(name_list)

5. pop

   name_list = ['Tom', 'Lily', 'Rose']

   del_name = name_list.pop(1)

   \# 结果：Lily

   print(del_name)

   \# 结果：['Tom', 'Rose']

   print(name_list)

6. remove

7. reverse 

   num_list = [1, 5, 2, 3, 6, 8]

   num_list.reverse()

   \# 结果：[8, 6, 3, 2, 5, 1]

   print(num_list)

8. index    name_list = ['Tom', 'Lily', 'Rose']  print(name_list.index('Lily', 0, 2)) # 1

9. count   name_list = ['Tom', 'Lily', 'Rose'] print(name_list.count('Lily')) # 1

10. copy

    name_list = ['Tom', 'Lily', 'Rose']

    name_li2 = name_list.copy()

    \# 结果：['Tom', 'Lily', 'Rose']

    print(name_li2)

11. extend

3、关键字不需要括号，函数（参数），方法（参数）方法通过对象调用。

4、列表应用场景：存储相同类型的数据，通过迭代遍历，在循环体内部，针对列表的每一项执行相同的操作

5、元组Tuple（元组的元素不能修改）

存储一串信息，数据间用，隔开

元组用（）定义，索引从0开始

6、字典dictionary

通常用于存储描述一个物体的相关信息

- 和列表的区别

  列表是有序的集合，字典是无序的集合

- 字典用{}定义

- 字典用键值对存储数据，键值对之间使用，隔开；key是索引，value是数据，键和值之间：，键是唯一，值可以是任何数据类型，键只能是字符串，数字或者元组

遍历key：dict1 = {'name': 'Tom', 'age': 20, 'gender': '男'}

for key in dict1.keys():

print(key)

遍历value：dict1 = {'name': 'Tom', 'age': 20, 'gender': '男'}

for value in dict1.values():

print(value)

遍历元素：dict1 = {'name': 'Tom', 'age': 20, 'gender': '男'}

for item in dict1.items():

print(item)

遍历键值对：dict1 = {'name': 'Tom', 'age': 20, 'gender': '男'}

for key, value in dict1.items():

print(f'{key} = {value}')

7、字符串string

一串字符，用一对双引号或单引号

索引获取一个字符串的指定位置的字符

for循环遍历字符串中的每一个字符

查找：find()：检测某个⼦子串串是否包含在这个字符串串中，如果在返回这个⼦子串串开始的位置下标，否则则返回-1。

修改：所谓修改字符串串，指的就是通过函数的形式修改字符串串中的数据。replace()：替换

8、切⽚片是指对操作的对象截取其中⼀一部分的操作。字符串串、列列表、元组都⽀支持切⽚片操作。

注：不包含结束位置下标对应的数据， 正负整数均可；步⻓长是选取间隔，正负整数均可，默认步⻓长为1。

eg：name = "abcdefg"

print(name[2:5:1]) # cde

print(name[2:5]) # cde

print(name[:5]) # abcde

print(name[1:]) # bcdefg

print(name[:]) # abcdefg

print(name[::2]) # aceg

print(name[:-1]) # abcdef, 负1表示倒数第⼀一个数据

print(name[-4:-1]) # def

print(name[::-1]) # gfedcba

9、条件语句：

- if 条件:

  条件成⽴立执⾏行行的代码1

  条件成⽴立执⾏行行的代码2

- if 条件:

  条件成⽴立执⾏行行的代码1

  条件成⽴立执⾏行行的代码2

  ......

  else:

  条件不不成⽴立执⾏行行的代码1

  条件不不成⽴立执⾏行行的代码2

- if 条件1：

  条件1成⽴立执⾏行行的代码

  条件1成⽴立执⾏行行的代码

  ​        if 条件2：

  ​        条件2成立执行的代码

  ​        条件2成立执⾏的代码

10、循环

while 条件:

条件成立重复执⾏的代码1

条件成立重复执⾏的代码2



break和continue是循环中满足一定条件退出循环的两种不同方式：

举例：一共吃5个苹果，吃完第一个，吃第二个…，这⾥里里"吃苹果"的动作是不是重复执行？

情况一：如果吃的过程中，吃完第三个吃饱了了，则不不需要再吃第4个和第五个苹果，即是吃苹果的动作

停⽌，这里就是break控制循环流程，即终止此循环。

情况二：如果吃的过程中，吃到第三个吃出一个大虫子...,是不是这个苹果就不吃了，开始吃第四个苹果，这里就是continue控制循环流程，即退出当前一次循环继而执行下一次循环代码。



for循环：

for 临时变量量 in 序列列:

重复执行的代码1

重复执⾏的代码2



11、函数1

定义：def 函数名(参数):

​                     代码1

​                     代码2

调用：函数名(参数)

函数的参数：函数调⽤用的时候可以传⼊入真实数据，增⼤大函数的使⽤用的灵活性

​	形参：函数定义时书写的参数(⾮非真实数据)

​	实参：函数调⽤用时书写的参数(真实数据)

函数的返回值可以返回给用户所需要的结果

函数嵌套：一个函数调用另一个函数

def testB():

​	print('---- testB start----')

​	print('这⾥里里是testB函数执⾏行行的代码...(省略略)...')

​	print('---- testB end----')

def testA():

​	print('---- testA start----')

​	testB()

​	print('---- testA end----')

testA()

12、函数2

变量作用域指的是变量生效的范围，主要分为两类：局部变量和全局变量。

​		局部变量：所谓局部变量是定义在函数体内部的变量，即只在函数体内部生效。局部变量的作用：在函数体内部，临时保存数据，即当函数调用完成后，则销毁局部变量。

​		全局变量：所谓全局变量，指的是在函数体内、外都能⽣效的变量。

返回值：return可退出当前函数，导致return后面的代码无法执行。

​				return a, b 写法，返回多个数据的时候，默认是元组类型。

​				return后⾯面可以连接列列表、元组或字典，以返回多个值。

位置参数：位置参数：调⽤用函数时根据函数定义的参数位置来传递参数。

关键字参数：通过“键=值”形式加以指定。函数调用时，如果有位置参数时，位置参数必须在关键字参数的前⾯面，但关键字参数之间不存在先后顺序。

缺省参数：缺省参数也叫默认参数，用于定义函数，为参数提供默认值，调用函数时可不传该默认参数的值（注意：所有位置参数必须出现在默认参数前，包括函数定义和调用）。

13、函数加强

递归：函数内部⾃己调⽤用⾃己，必须有出口

```python
# 3 + 2 + 1
def sum_numbers(num):
# 1.如果是1，直接返回1 -- 出⼝口
if num == 1:
return 1
# 2.如果不不是1，重复执⾏行行累加:
result = num + sum_numbers(num-1)
# 3.返回累加结果
return result
sum_result = sum_numbers(3)
# 输出结果为6
print(sum_result)
```



lambda表达式：如果一个函数有一个返回值，并且只有⼀句代码，可以使用 lambda简化。

```
lambda 参数列列表 ： 表达式
```

lambda表达式的参数可有可无，函数的参数在lambda表达式中完全适用。

lambda函数能接收任何数量的参数但只能返回一个表达式的值

```
# 函数
def fn1():
return 200
print(fn1)
print(fn1())
# lambda表达式
fn2 = lambda: 100
print(fn2)
print(fn2())

#lambda实现
print((lambda a, b: a + b)(1, 2))
```

高阶函数：把函数作为参数传入，这样的函数称为⾼阶函数

map()

map(func, lst)，将传⼊的函数变量func作用到lst变量的每个元素中，并将结果组成新的列列表(Python2)/迭代器器(Python3)返回。

需求：计算list1 序列中各个数字的2次⽅。

```
list1 = [1, 2, 3, 4, 5]
def func(x):
return x ** 2
result = map(func, list1)
print(result) # <map object at 0x0000013769653198>
print(list(result)) # [1, 4, 9, 16, 25]
```

reduce()

reduce(func(x,y)，lst)，其中func必须有两个参数。每次func计算的结果继续和序列的下⼀个元素做累积计算。

注意：reduce()传⼊的参数func必须接受2个参数。

需求：计算list1 序列中各个数字的累加和。

```
import functools
list1 = [1, 2, 3, 4, 5]
def func(a, b):
return a + b
result = functools.reduce(func, list1)
print(result) # 15
```

filter()

filter(func, lst)函数⽤于过滤序列, 过滤掉不符合条件的元素, 返回一个 filter 对象,。如果要转换为列表,可以使用 list() 来转换。

```
list1 = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
def func(x):
return x % 2 == 0
result = filter(func, list1)
print(result) # <filter object at 0x0000017AF9DC3198>
print(list(result)) # [2, 4, 6, 8, 10]
```

