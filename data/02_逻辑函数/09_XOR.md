# XOR

## 语法

**XOR**(布尔值 1,[布尔值 2...布尔值 254])  
**XOR**(logical1,[logical2...logical254])

### 参数

1. 布尔值

## 概述

当奇数个参数为 TRUE 或 非 0 数值 时返回 TRUE，偶数个参数为 TRUE 或 非 0 数值 时返回 FALSE。

## 示例

```excel
XOR(1)
```

输出：  
TRUE

---

```excel
XOR(1,TRUE)
```

输出：  
FALSE

---

```excel
XOR(0,TRUE,1,1=1,FALSE)
```

输出：  
TRUE
