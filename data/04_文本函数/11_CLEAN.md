# CLEAN

## 语法

**CLEAN**(文本)  
**CLEAN**(text)

### 参数

1. 待处理的文本。

## 概述

删除文本中不可见字符(ASCⅡ 字符集)。

## 示例

```excel
CLEAN(CHAR(9)&"Hello World"&CHAR(10))
```

返回：  
"Hello World"
