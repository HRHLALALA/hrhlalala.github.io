---
title: Python Style
date: '2020-09-12'
excerpt: >-
 This is the python style
layout: post
--- 

### 变量命名规则
#### 1. 每一个变量命名时使用一种规则：
```
b（单个小写字母）
B（单个大写字母）
lowercase
lower_case_with_under_scores
UPPCASE
UPPERCASE_WITH_UNDERSCORES
CaptilizedWorkds (驼峰写法,首字母大写）
mixedCase(驼峰写法,首字母小写）

拒绝：
Capitalized_Words_With_Underscore
```

#### 2. 尽量统一一种自然语言，除非情况特殊尽可能使用英语：

```python
接受
is_binary = True
 
拒绝
is_er_jin_zhi = True
shi_er_jin_zhi = True
```


#### 3. 有描述性, 尽可能少用缩写
接受以下命名
```python
price_tag = "$500" #标价500元
num_errors = 100   #100个错误，num是number的缩写，通用
is_connected = True #是否连接
```

遇到数据结构的时候，可以描述在变量名里
```python
book_list = [book1,book2]
book_tuple = (book1,book2)

#当然也可以使用books = [book1,book2],但是这样看不出来是什么类型，因此book_list更好。
```

拒绝以下命名

```python
l = 1 或 I = 1 或 o = 0
n = 0 # n可以用在很多地方，但没有意义，没有描述性

nerr = 100 #含糊不清的缩写
pc_reader = ... # pc有太多意思
cstmr_id = 0 #原意是customer id，但是删除太多字，最好使用customer_id

connected = True
#connected 可以有很多种理解，如过去连接的东西。is_connected 确定变量类型是boolean

```

#### 4. 不要使用过长的变量名
20个字符以内, 少于4个单词
拒绝
```
doYouThinkThisIsAGoodVariableName
```

#### 5. 不要使用一些常用的函数名作为变量名
拒绝：
```python
int = 10
str = "hello" # str()就没有意义
```

#### 6. for循环中的情况

接受：
```python
for i in range： # i 是index的缩写
```
避免：
```python
for i in list: # 用具体元素的描述 如 for book in books：
for x in range：# x毫无意义
```

#### 7. 一些程序员之间的命名习惯
普通变量首字母小写,使用lower_case_with_under_scores的写法
```python
dog_name = "Tom"
age = 10
```

函数名首字母小写，使用lower_case_with_under_scores或mixedCase

```python
def play_game():
    ...
    
def playGame():
    ...

两种都可以接受，优先使用第一种
    
```
class名首字母大写，使用CapCase
```python
class GameController:
    ...
```

隐藏变量或隐藏函数：如果不想被import的函数，或在class里表示private variable，名字前加下划线_
```python
# 在file 1 里
def _shuffle_card(..):
    ...
    
def replay(...):
    _shuffle_card(..)
  
# 在file 2 里  
    
from file1 import replay # 规定不要import _shuffle_card
```

常量constant variable使用全大写
```python
BRAND_NAME = "Apple"
COMPANY_LOCATION = "..."
```


Exception,变量名后面 + Error

```python
class RunTimeError
```


### 缩进

#### 1. 使用4 space 缩进
接受
```python
for i in range(10):
    print(i)
``` 
拒绝
```python
for i in range(10):
  print(i)
``` 

#### 2. tab vs space
1. 优先使用space
2. 如果全文都是tab，那就使用tab

#### 3. 括号里的参数换行，参数对齐括号或超过括号
接受
```python
def long_function_name(var_one,var_two,
                        var_three,var_four):       
```
拒绝
```python
def long_function_name(var_one,var_two,
    var_three,var_four):       
```

#### 4. 如果括号里的参数从新的一行开始，参数需多加一次缩进
接受
```python
def long_function_name(
        var_one,var_two,
        var_three,var_four):
    print(var_one)
               
```
拒绝
```python
def long_function_name(
    var_one,var_two,
    var_three,var_four):
    print(var_one)               
```

#### 5. 如果是if语句，为了视觉上的清晰，可以接受不多加缩进

接受
```python
if (it_is_condition_1 and
    it_is_condition_2):
    do_something()
 
或   
    
if (it_is_condition_1 and
    it_is_condition_2):
    # function description 多加一行注释可以更清晰
    do_something()
               
或
if (it_is_one_thing
        and it_is_another_thing):
    do_something()     
```

#### 6. list
```python
board = [
        1,2,3,
        4,5,6,
        7,8,9]
        
或

board = [
    1,2,3,
    4,5,6,
    7,8,9,
]
```

#### 7. 什么时候需要换行
一行限制72个字，为了能够多窗口打开

### 关于import

#### 1. 不要连续import不同的包,可以从同一个包中连续import东西
接受：
```python
import sys
import os
from tkinter import Button, Label
```
    
拒绝：
```python
import sys，os
```

#### 2. 尽量使用绝对import 
提倡
```python
import mymodule.fun1

from mymodule import fun1
from mymodule.fun1 import fun1_1
```

避免, 但是复杂情况中可以接受

```python
from . import fun1
from .fun1 import fun1_1
```


#### 3. 避免import *
import * 会引入一系列不必要的内容


### 代码中的空格

#### 1. 括号后面，前面不要空格

接受：
```python
play_game(game_name)
```

拒绝：
```python
play_game( game_name )
```

#### 2.逗号和括号之间不要空格

接受：
```python
num_list = [1,]
```

拒绝：
```python
num_list = [1, ]
```

#### 3. 逗号，冒号，分号前不要空格
接受：
```python
if x == 4:
    x, y = y, x
```

拒绝：
```python
if x == 4 : 
    x , y = y , x
```

#### 4. 逗号，冒号，分号前不要空格
接受：
```python
if x == 4:
    x, y = y, x
```

拒绝：
```python
if x == 4 : 
    x , y = y , x
```

#### 5. 在list里的冒号有以下规则
接受：
```python
book_list[1:9], book_list[1:9:3],book_list[1::9]
book_list[lower:upper]
book_list[lower+offset : upper+offset]
book_list[lower + offset : upper + offset]
book_list[: some_index : some_index】
```

拒绝：
```python
book_list[1: 9], book_list[1:9 :3],book_list[1: :9]
book_list[lower : : upper]
book_list[ : some_index : some_index]

```

#### 6.函数调用的时候，函数名和括号之间不要空格
接受
```python
my_function()
```
拒绝
```python
my_function ()
```

#### 7.作为index的[]前不要有空格
接受
```python
my_list[1]
```
拒绝
```python
my_list [1]
```

#### 8.运算符前后不要有超过1个空格
接受
```python
x = 1
y = 2
```
拒绝
```python
x     =1
y     =1
```

#### 9.运算符前后最好有一个空格
接受
```python
z = (x + y) * (x - y)
z += 1
```
拒绝
```python
z=(x+y)*(x-y)
z+=1
```

#### 10.函数参数里设置默认值的=号前后不要有空格
接受
```python
def my_function(a, b=1):
    ...
```
拒绝
```python
def my_function(a, b = 1):
    ...
```

但是如果有参数注释，可以使用空格
```python
def my_function(a, b: AnyStr = ""):
    ...
```

### 注释
#### 1. 注释应该是要完整的句子
接受
```python
width += 1 # 增加宽度
```
拒绝
```python
width += 1 # 加一
```

#### 2. 注释应该是说明代码在整段代码的作用
接受
```python
width = 20  #设置长方形的初始宽度
num_apples = 20 # 一开始有20个苹果（解释num的意思）
```
拒绝
```python
width = 20 #宽度为20
num_apples = 20 # 设置变量num_appls为20
```

#### 3. 介绍参数含义
```python
def my_function(param1,param1, ....):
    """
    这个函数用来...
    
    参数param1: ...
    参数param2: ...
    参数param3: ...
    ...
    
    返回值result:
    """
    do_something(param1, param2)
    ...
    return result
    
```
调用的时候
```python
my_function(
    param1, #...
    param2, #...
    ....
)
```




#### 4. 文件内容注释
放文件开头

模块文件：
```python
"""
这个文件为music player的一些必要的函数
例：
    from music_player import play_music, ...
    mixer = ..
    play_music(mixer)
"""
```

主文件：
```python
"""
项目名：
作者：
时间：

项目介绍：
"""
```

#### 5. 复杂,或抽象的代码的注释
```python
"""
用户切换play按钮时候改变play的显示内容：
播放的时候显示暂停，暂停的时候显示播放
"""
if music.is_playing:
    play_btn.config(text="pause")
else:
    play_btn.config(text="play")

```

或
```python
"""
用户切换play按钮时候改变play的显示内容：
播放的时候显示暂停，暂停的时候显示播放
"""
if music.is_playing:
    #更新歌词，显示,....
    ...
    
else:
    #时间更新停止

```

#### 6. TODO
如果函数是即将要编写的，或者要分配给队友做，可以注释TODO
```python
def my_function(param):
    #TODO: 函数功能介绍
    pass
    
def your_function(param):
    #TODO: 函数功能介绍
    #Assign： 交给谁做
    pass    
    
```

#### 7. 其他：
1. 如果项目很复杂，注释可以让你快速理解代码
2. 注释要简洁明了
3. 注释也要让其他人看得懂，因为队友需要阅读你的代码
4. 注释不要太乱，太乱会看的很累





