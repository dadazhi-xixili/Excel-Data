# ISERR
## 语法
**ISERR**(值)	    
**ISERR**(value)


### 参数
1. 值 value ：检验的值
## 概述
判断传入值是否为非#N/A的错误值。
## 示例
```
ISERR(NA())
输出：
FALSE

ISERR(1/0)
输出：
TRUE

ISERR(TRUE)
输出：
FALSE


ISERR(1)
输出：
FALSE
```