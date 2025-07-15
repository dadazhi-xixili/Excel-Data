# ISREF
## 语法
**ISREF**(引用)	    
**ISREF**(reference)


### 参数
1. 引用 reference ：检验的值
## 概述
判断传入值是否为引用。
## 示例
```
ISREF(A1)
输出：
TRUE

ISREF(A1:C3)
输出：
TRUE

ISREF(XLOOKUP(1,{1,2},A1:B1))
输出：
TRUE

ISREF(1)
输出：
FALSE

ISREF(TRUE)
输出：
FALSE

```