# AND

## 语法

**AND**(布尔值 1[,布尔值 2...布尔值 255])  
**AND**(logical1[,logical2,...logical255])

### 参数

1. 布尔值 logical：TRUE 或 FALSE 或数值。

## 概述

判断所有参数是否都为 TRUE 和非零数值。

### 常见错误

1. 输入不包含布尔值和数值则返回#VALUE!。

## 示例

```excel
AND(TRUE,1,TRUE)
```

输出：  
TRUE

---

```excel
AND(TRUE,TRUE,FALSE)
```

输出：  
FALSE

---

```excel
AND(TRUE,0)
```

输出：  
FALSE
