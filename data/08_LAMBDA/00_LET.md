# LET

## 语法

**LET**(名称 1,表达式 1[,名称 2,表达式 2,...],返回)  
**LET**(name1,calculation1[,name2,calculation2,...],output)

### 参数

1. 名称 name：定义变量的名称。
2. 表达式 calculation1：定义变量的计算公式。
3. 返回 output：返回的计算结果。
4. 名称 n name_n: 多个变量名称。
5. 表达式 n calculation_n: 多个变量的计算公式。

## 概述

定义多个变量，并返回计算结果。  
可重复使用变量结果，避免重复计算。

### 常见错误

1. 名称必须是唯一。
2. 名称与表达式必须成对。
3. 定义名称不能与已有的环境名称冲突，如 A1、函数名、名称管理器中的名称等。

## 示例

### 示例 1

```excel
LET(x,1,y,2,z,x+y,z*x*y)
```

```excel
计算过程：
LET(x,1,y,2,z,1+2,z*x*y)
LET(x,1,y,2,z,3,x*y*z)
LET(x,1,y,2,z,3,1*2*3)
6
```

### 示例 2

```excel
LET(f,LAMBDA(x,y,x+y),f(1,2))
```

```excel
计算过程
LAMBDA(x,y,x+y)(1,2)
1+2
3
```
