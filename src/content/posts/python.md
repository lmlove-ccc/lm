---
title: Python语法基础（一）
published: 2025-12-07
description: python学习【基于兴趣爱好】
tags: [python]
category: 编程
draft: false
---
# 基于python的学习指导
## 1.print（）函数具有以下功能
 > #### *  打印（）中的任何字符 均有严格的要求
   >若（）中为**字符串** 则必须要有变量被**赋值** 
   >* 如 **“hello ward”** 等

### print（）函数具体效果如下
~~~ python
a = '11月05日'#a为字符串str
 print(a)
~~~
其输出结果为 **11月05日**
### print函数中不难免有些已经预定好的函数
**如 ‘sep’ ‘end’等**
* sep函数
  >可看作为分隔符
* end函数
  >可看作为调整下一行的符号
#### 其效果如下
~~~python
a = '你好'#a为字符串str
b = 'py'
 print(a,b,sep=',',end='!' )
 ~~~
 其输出结果为**你好,py!**
 ## 2.数据类型
### int为整型  float为浮点型  bool为布尔型常用来做判断 complex为复数型 字符串str
>str
    > * 上述中 a b 皆为str

>int
    > * 自然数如 0 1 2 3 4 等（-1 -2 -3等 也算）

>float
    > * 小数如 1.1 1.2 1.3等（负数也可以）

>bool
    > * True与False **注**首字母为**大写**

>cpmplex
    > * m = 1+2j   
1为实部 2j为虚部 j为虚部单位 **注 虚部单位 字母表示只能为 j**

## 3.type函数
**做为判断数据类型的函数**

效果如下
~~~python
num = 1
num2 = 1.2
print(type(num),type(num2),type(True),sep='/', end='!')
~~~
其输出为 **'int'/ 'float'/ 'bool'!**
## 4.input函数
**做为输入函数**

效果如下
~~~python
input("请输入内容")
~~~
其输出为 **请输入内容**

### 当然
也可以为input进行赋值 并与print共用
~~~python
N = input("请输入内容")
print(N)
~~~
其输出为 **请输入内容**
> 在其输出后可填写内容 （任意） 之后 回车 便会输出内容
## 转义字符
> ### 1. \t 制表符 通常空四个字符
    > * 例如
~~~python
print("姓名\t年龄\t电话")
~~~
其输出为 **姓名	年龄	电话**
> ### 2. \n 换行符
    > * 例如
~~~python
 print("姓名\n年龄\n电话")
 ~~~
 其输出为

 **姓名**

 **年龄**

 **电话**
 > ### 3. \r 回车 表示将当前位置移至本行开头
~~~python
  print("姓名\r年龄\t电话")
~~~
其输出为 **年龄 电话**
> ### 4. \f 反斜杠符
~~~python
  print("姓名\\f年龄")
~~~
其输出为 **姓名年龄**
> ### 5. r 取消转义
~~~python
  print(r"姓名\r年龄")
~~~
其输出为 **姓名\r年龄**
## if 判断
判断条件 if 内容：
例如
~~~python
age = 10
if age < 18:
    print('年龄不符合')
~~~
其输出为 **年龄不符合**    
## 运算符
> ### 1.比较运算符
> * == **比较两个值是否相等**
> * != **与==恰恰相反**
> * <与> **均比较两个值是否相等**
> ### 2.逻辑运算符
> * and **左右两边都符合才为true**
> * or **左右两边一边符合就为true**
> * not **表示相反的结果**
> ### 三目运算
> * if
> * else **其后面不需要添加任何条件**
## 基本格式
> if-else
> * if 条件：
>
>    满足条件要做的事
>
>    else：
>
>   不满足条件要做的事

**例如**
~~~python
a = 1
if a == 1:
    print('true',end = " ")
else:
    print('false')
if a == 2:
        print('true',end = " ")
else:
        print('false')
~~~
其输出为 **true**   **false**