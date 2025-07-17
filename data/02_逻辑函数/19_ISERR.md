# ISERR

## 语法

**ISERR**(值)  
**ISERR**(value)

### 参数

1. 值 value ：检验的值

## 概述

判断传入值是否为非#N/A 的错误值。

## 示例

```excel
ISERR(NA())
```

返回：  
FALSE

---

```excel
ISERR(1/0)
```

返回：  
TRUE

---

```excel
ISERR(TRUE)
```

返回：  
FALSE

---

```excel
ISERR(1)
```

返回：  
FALSE
