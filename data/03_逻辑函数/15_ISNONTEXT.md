# ISNONTEXT
## 语法
**ISNONTEXT**(值)	    
**ISNONTEXT**(value)


### 参数
1. 值 value ：检验的值
## 概述
判断传入值是否非文本。
## 示例
```
ISNONTEXT("1")
输出：
FALSE

ISNONTEXT("")
输出：
FALSE

ISNONTEXT(1)
输出：
TRUE

ISNONTEXT(FALSE)
输出：
TRUE
```