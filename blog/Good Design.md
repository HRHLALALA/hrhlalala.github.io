---
title: Good Design - Python (Chinese)

date: '2020-09-19'
thumb_image: images/code-smell.png
image: images/code-smell.png
excerpt: >-
 This blog concludes how to distinguish bad designs and how to reconstruct them. It is suitable for beginners who haven't learnt OOP yet. It was used to be instructed to my Python students because they were designing software application by themselves. 
layout: post
--- 

## Code Smells 代码异味
### 1. Duplicated Code 代码重复

#### 例子

已经写过类似的Python代码，但是没有放在函数里，所以能难使用
```python
import turtle

t = turtle.Pen()
t.pensize(5)
#1绿色枝干
t.color("green")
t.left(90)
t.forward(50)
#2蓝色叶子
t.color("blue")

#两片叶子
for i in range(2):
    for j in range(15):
        t.forward(5)
        t.right(6)
    t.right(90)
    
#3紫色枝干
t.color("purple")
t.forward(150)
#4红色的花
t.color("red")
# 花
for i in range(6):
    for i in range(2):
        for j in range(15):
            t.forward(5)
            t.right(6)
        t.right(90)
    t.left(60)
```

解决方案： 把重复的部分放入函数调用
```python
import turtle

#绘制叶子的函数
def draw_leaf():
    for i in range(2):
        for j in range(15):
            t.forward(5)
            t.right(6)
        t.right(90)

t = turtle.Pen()
t.pensize(5)
#1绿色枝干
t.color("green")
t.left(90)
t.forward(50)
#2蓝色叶子
t.color("blue")
draw_leaf()
#3紫色枝干
t.color("purple")
t.forward(150)
#4红色的花
t.color("red")
for i in range(6):
    draw_leaf()
    t.left(60)
```

已经写过类似功能的函数，但是需要修改后才能使用，但是函数没有办法修改

```python
def init_board():
    # initialize 3x3 board
    
    board = []
    for i in range(3):
        row = []
        for j in range(3):
            row.append(0)
        board.append(row)
    
 # 一段很长的代码都需要init_board_3....但是用户说需要5x5的盘，于是
    
board = []
for i in range(5):
    row = []
    for j in range(5):
        row.append(0)
    board.append(row) 
...
```

解决方案：
```python
def init_board(board_size):
    # initialize 3x3 board
    
    board = []
    for i in range(board_size):
        row = []
        for j in range(board_size):
            row.append(0)
        board.append(row)    
init_board(3)
...
init_board(5)
...

```

#### 例子
已经写过类似功能的函数，但是只需要其中一部分
```python
# 2048.py

import random

def init_board():
    # 新建空白棋盘，随机两个位置放入2或4
    board = []
    for i in range(4):
        row = []
        for j in range(4):
            row.append(0)
        board.append(row)
        
    
    for y in range(2):
        while True:
            choice=[2,4]
            i=random.randint(0,3)
            j=random.randint(0,3)
        
            if board[i][j]!=0:
                pass
            else:
                board[i][j]=random.choice(choice)
                    break
    return board
    
...

# 现在更改了游戏规则，需要增加全部都是2的棋盘
board = []
for i in range(4):
    row = []
    for j in range(4):
        row.append(2)
    board.append(row)
...

```
重构后：
```python
# 2048.py

import random

def init_board(size,init_num = 0):
    # 新建空白棋盘，随机两个位置放入2或4
    board = []
    for i in range(size):
        row = []
        for j in range(size):
            row.append(init_num)
        board.append(row)

def init_random_positions(board):   
    for y in range(2):
        while True:
            choice=[2,4]
            i=random.randint(0,len(board)-1)
            j=random.randint(0,len(board)-1)
        
            if board[i][j]!=0:
                pass
            else:
                board[i][j]=random.choice(choice)
                    break
    return board
    
...

# 现在更改了游戏规则，需要增加全部都是2的棋盘
board = init_board(4,init_num = 2):
...

```

### 解决方案
* 将重复的代码放入函数
* 设置重要的参数
* 拆分函数，让函数能适应各种情况

### 2. 长函数

* 因为写代码比读代码容易，所以在方法变成一个丑陋的、巨大的庞然大物之前是感觉不到的
* “代码只有两行，为它创建一个完整的函数是没有意义的……”这意味着又加了一行又一行，产生了一堆乱七八糟的代码

#### 例子

```python
t = turtle.Pen()
t.pensize(5)
t.left(90)

def draw_leaf():
    for i in range(2):
        for j in range(15):
            t.forward(5)
            t.right(6)
        t.right(90)

def draw_flower():
    #1绿色枝干
    t.color("green")
    t.forward(50)
    #2蓝色叶子
    t.color("blue")
    draw_leaf()
    #3紫色枝干
    t.color("purple")
    t.forward(150)
    #4红色的花
    t.color("red")
    for i in range(6):
        draw_leaf()
```

#### 解决方案
* 拆分函数
* 尝试给代码加上注释 

```python
t = turtle.Pen()
t.pensize(5)
t.left(90)
    
def draw_leaf(color):
    t.color(color)
    for i in range(2):
        for j in range(15):
            t.forward(5)
            t.right(6)
        t.right(90)

def draw_branch(color,length):
    # 枝干
    t.color(color)
    t.forward(length)
 
def draw_petal(color,petal_num):
    # 花瓣
    for i in range(petal_num):
        draw_leaf()
        t.left(360/petal_num)
   
def draw_flower():
    
    #1绿色枝干
    draw_branch("green", 50)
    
    #2蓝色叶子
    draw_leaf("blue")
    
    #3紫色枝干
    draw_branch("purple",150)
    
    #4红色的花
    draw_petal("red", 6)
```


### 3. Divergent Change 发散式变化
* 当添加一个新功能的时候，需要修改很多地方
* 添加新的功能会很困难
* 通常发生在添加新功能的时候

#### 例子
```python
def taste1():
    something()
...
def tasteN():
    something()
    
def smell1():
    something()
...
def smellN():
    something()


def taste(fruit_name):
    if fruit_name == "apple":
        taste1()
    elif fruit_name == "pear":
        taste2()
    elif fruit_name == "watermelon":
        taste3()
    elif ...
        tasteN()

        
def smell(fruit_name):
    if fruit_name == "apple":
        smell1()
    elif fruit_name == "pear":
        smell2()
    elif fruit_name == "watermelon":
        smell3()
    elif ...
        smellN()



fruit_name = "apple"

```

如果`fruit_name` 换成其他水果，就需要对这些函数都添加一遍

#### 解决方案
避免使用这类一连串 if 语句
```python


def taste1():
    something()
def smell1():
    something()

def taste(fruit):
    fruit['taste']()
    

        
def smell(fruit):
    fruit['smell']()

fruit = {
    "name": "apple",
    "taste":  taste1,
    "smell": smell1,
}


```


### 4. Shotgun Surgery 霰弹枪手术
* 当修改一个函数的时候，其他函数都要跟着修正
* 通常Debug的时候
* 危害
    * 增加开发人员的工作量
    * 代码的潜在疏忽

#### 例子
```python
# 原要求：每个函数你都需要检测 money 不能小于0且不能超过1000

def save_money(money):
    if money < 0 or money > 1000:
        print("money can only in range between 0 and 1000")
    else:
        _here_save_money()
        
def transfer_money(money,target):
    if money < 0 or money > 1000:
        print("money can only in range between 0 and 1000")
    else:
        _transfer_money()
    
....


# 新要求：money 不能小于0且不能超过500 而且money不等于100
# 这样就需要重新修改这些函数
      
```
#### 解决方案
拆分函数，把公共部分拿出来

```python
# 要求：money 不能小于0且不能超过500 而且money不等于100，
rule = {
    "lower_bound":0,
    "upper_bound":1000,
    "sensitive_values":100,
}
def print_rule_invalid_msg(rule):
    print("cannot in range",rule['lower_bound'], "and", ...)
    
def check_money_validation(money, rule = rule):
    if (money < rule['lower_bound'] or 
        money < rule['upper_bound'] or 
        money == rule['sensitive_values']):
        # start
        print_rule_invalid_msg(rule)
        return False
    else:
        return True
        

def save_money(money):
    if check_money_validation(money):
        _here_save_money()
        
def transfer_money(money,target):
    if check_money_validation(money)
        _transfer_money()
      
```
如果可能需要应对不同的情况 仿Strategy Pattern
```python
def check_upper_lower_bound(moneey,lower,upper):
    if money< lower or money > upper:
        return False
    else:
        return True
def check_sensitive_amounts(moneey,amounts):
    if money in amounts:
        return False
    else:
        return True   
             
def print_rule_invalid_msg(rule):
    """
    Some code here
    """
    print(...)
   
"""
例：假如Money 不能在区间100-150，300-350之内，且不能等于120 和170
"""    
rules = [
    lambda money: check_upper_lower_bound(money,100,150),
    lambda money: check_upper_lower_bound(money,300,350),
    lambda money: check_sensitive_amounts(money,[120,170]),   
]
  
def check_money_validation(money,rules):
    for rule in rules:
        if not rule():
            return False
    return True
            
        

def save_money(money):
    """
    init rules here
    """
    if check_money_validation(money,rules):
        _here_save_money()
        
def transfer_money(money,target):
    """
    init rules here
    """
    if check_money_validation(money,rules)
        _transfer_money()
      
```

### 5. Long Parameter List 长参数群
* 函数的参数过多
* 在将几种类型的算法合并到一个方法中之后，可能会出现一长串参数
* 参数传递会很困难，容易出错
* 不容易Debug
* 

#### 例子：
```python

def draw_flower(    
                    upper_left_point,
                    lower_right_point,
                    lower_branch_color,
                    lower_branch_length,
                    leaf_color,
                    leaf_length,
                    upper_branch_color,
                    upper_branch_length,
                    petal_color,
                    petal_num,
                    pen_size, 
                    )：
    
    t.pensize(pen_size)
    
    #----------------
    # 画笔归位代码
    #----------------
    
    #1绿色枝干
    draw_branch(lower_branch_color, lower_branch_length)
    
    #2蓝色叶子
    draw_leaf(leaf_color,leaf_length)
    
    #3紫色枝干
    draw_branch(upper_branch_color,upper_branch_length)
    
    #4红色的花
    draw_petal(petal_color, petal_num)
 
def draw_flowers(
                num_flowers,
                upper_left_point,
                lower_right_point,
                lower_branch_color,
                lower_branch_length,
                leaf_color,
                leaf_length,
                upper_branch_color,
                upper_branch_length,
                petal_color,
                petal_num,
                pen_size):  
    for i in range(num_flowers)               
        draw_flower(
                upper_left_point,
                lower_right_point,
                lower_branch_color,
                lower_branch_length,
                leaf_color,
                leaf_length,
                upper_branch_color,
                upper_branch_length,
                petal_color,
                petal_num,
                pen_size
        )
        # some code to adjust direction
    # some code to do with flowers
```

原来设想upper_left_point和lower_right_point作为花的bounding box的位置，但是发现代码与愿相违

如果需要将upper_left_point, lower_right_point 换成起始点x，y怎么办

### 解决方案
在python 中可以使用 *args或**kwarg的方法，或者设定默认值
```python
flower_config = {
    "num_flowers": 6,
    "upper_left_point": (0,0),
    "lower_right_point":(20,20),
    "lower_branch_color":"green",
    "lower_branch_length": 50,
    "leaf_color":"yellow",
    "leaf_length":10,
    "upper_branch_color": "purple",
    "upper_branch_length": 150,
    "petal_color": "purple",
    "petal_num":6 ,
    "pen_size":5
    
}
    
def back_to_position(x,y):
    somecode()
    
def draw_flower(**configs)：
    
    t.pensize(configs.pen_size)
    
    back_to_position()
    
    #1绿色枝干
    draw_branch(configs.lower_branch_color, configs.lower_branch_length)
    
    #2蓝色叶子
    draw_leaf(configs.leaf_color,configs.leaf_length)
    
    #3紫色枝干
    draw_branch(configs.upper_branch_color,configs.upper_branch_length)
    
    #4红色的花
    draw_petal(configs.petal_color, configs.petal_num)

def draw_flowers(num_flowers,**flower_configs):
    for i in range(num_flowers):            
        draw_flower(follow_configs)
        
draw_flowers(6, flower_configs)        
```

### 6. Function Chains 信息链
* A函数调用B函数，B函数调用C函数,...
* 如果一个比较深的函数出现问题，其他都会影响
* Debug 困难


#### 例子
```python
def cal_common_factors(a,b):
    #------------
    # Some code to calculate common factors
    #------------
    return common_factors
    
def cal_common_factors_3(a,b,c)
    common_factors = []
    for common_factor in cal_common_factors(a,b):
        common_factors.append(common_factors(c,common_factor))
        
    return common_factors
    
def cal_common_factors_4(a,b,c,d):
    common_factors = []
    for common_factor in cal_common_factors_3(a,b,c)
        common_factors.append(common_factors(d,common_factor))
        
    return common_factors
```

#### 解决方案
```python
def cal_common_factors_2(a,b):
    #------------
    # Some code to calculate common factors
    #------------
    return common_factors
    
def cal_common_factors(*args):
    #------------
    # Some code to calculate common factors using cal_common_factors_2
    #------------
    dosomething()
    


```