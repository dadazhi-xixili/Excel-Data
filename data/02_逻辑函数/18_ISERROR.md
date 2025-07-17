# ISERROR

## 语法

**ISERROR**(值)  
**ISERROR**(value)

### 参数

1. 值 value ：检验的值

## 概述

判断传入值是否为错误值。

## 示例

```excel
ISERROR(NA())
```

返回：  
TRUE

---

```excel
ISERROR(1/0)
```

返回：  
TRUE

---

```excel
ISERROR(TRUE)
```

返回：  
FALSE

---

```excel
ISERROR(1)
```

返回：  
FALSE
