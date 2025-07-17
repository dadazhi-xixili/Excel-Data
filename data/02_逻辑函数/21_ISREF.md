# ISREF

## 语法

**ISREF**(引用)  
**ISREF**(reference)

### 参数

1. 引用 reference ：检验的值

## 概述

判断传入值是否为引用。

## 示例

```excel
ISREF(A1)
```

返回：  
TRUE

---

```excel
ISREF(A1:C3)
```

返回：  
TRUE

---

```excel
ISREF(XLOOKUP(1,{1,2},A1:B1))
```

返回：  
TRUE

---

```excel
ISREF(1)
```

返回：  
FALSE

---

```excel
ISREF(TRUE)
```

返回：  
FALSE
