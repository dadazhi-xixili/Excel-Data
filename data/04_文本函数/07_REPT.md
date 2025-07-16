# REPT

## 语法

**REPT**(文本,次数)  
**REPT**(text,number_times)

### 参数

1. 文本 text：重复的文本。
2. 次数 number_times：重复的次数。

## 概述

重复文本指定次数。

### 补充

1. 次数会向下截取为整数。

## 示例

```excel
REPT("Hello",3)
```

输出：  
"HelloHelloHello"

```excel
REPT("Hello",0.9)
```

输出：  
""
