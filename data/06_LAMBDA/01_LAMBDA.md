# LAMBDA
## 语法
**LAMBDA**([参数1,参数2,...],表达式)        
**LAMBDA**([parameter1,parameter2,...],calculation)
### 参数
1. 参数 parameters：参数列表，参数用英文逗号隔开。    
接受数值、文本、日期、时间、布尔值、公式、引用、函数等任意数据类型。
2. 表达式 calculation：计算公式。
## 概述
创建一个函数，该函数可以接受参数并返回计算结果。主要应用场景是封装一个复杂的计算公式，方便后续重复使用。
## 示例
### 示例1
```excel
LAMBDA(x,SUM(SEQUENCE(x)))(10)
计算过程：
=SUM(SEQUENCE(10))
=SUM({1;2;3;4;5;6;7;8;9;10})
=55
```
### 示例2
```excel
=LET(
fxa,LAMBDA(x,y,x*y),
fxb,LAMBDA(
    x,y,
    f_1,f_2,
    f_1(x,y)+f_2(x,y)
),
fxb(2,3,fxa,SUM)
)
计算过程：
=fx2(2,3)
=fx1(2,3)+SUM(2,3)
=2*3+2+3
=11
```