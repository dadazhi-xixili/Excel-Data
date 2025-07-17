# ISNA

## 语法

**ISNA**(值)  
**ISNA**(value)

### 参数

1. 值 value ：检验的值

## 概述

判断传入值是否为#N/A。

## 示例

```excel
ISNA(NA())
```

返回：  
TRUE

---

```excel
ISNA(1/0)
```

返回：  
FALSE

---

```excel
ISNA(TRUE)
```

返回：  
FALSE

---

```excel
ISNA(1)
```

返回：  
FALSE
