# ISERROR

## 语法

**ISERROR**(值)  
**ISERROR**(value)

### 参数

1. 值 value ：检验的值

## 概述

判断传入值是否为错误值。

## 示例

```
ISERROR(NA())
输出：
TRUE

ISERROR(1/0)
输出：
TRUE

ISERROR(TRUE)
输出：
FALSE


ISERROR(1)
输出：
FALSE
```
