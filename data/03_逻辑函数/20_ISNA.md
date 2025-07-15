# ISNA
## 语法
**ISNA**(值)	    
**ISNA**(value)


### 参数
1. 值 value ：检验的值
## 概述
判断传入值是否为#N/A。
## 示例
```
ISNA(NA())
输出：
TRUE

ISNA(1/0)
输出：
FALSE

ISNA(TRUE)
输出：
FALSE


ISNA(1)
输出：
FALSE
```