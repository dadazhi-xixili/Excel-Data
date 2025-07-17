# ISNONTEXT

## 语法

**ISNONTEXT**(值)  
**ISNONTEXT**(value)

### 参数

1. 值 value ：检验的值

## 概述

判断传入值是否非文本。

## 示例

```excel
ISNONTEXT("1")
```

返回：  
FALSE

---

```excel
ISNONTEXT("")
```

返回：  
FALSE

---

```excel
ISNONTEXT(1)
```

返回：  
TRUE

---

```excel
ISNONTEXT(FALSE)
```

返回：  
TRUE
