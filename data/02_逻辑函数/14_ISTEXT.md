# IFTEXT

## 语法

**ISTEXT**(值)  
**ISTEXT**(value)

### 参数

1. 值 value ：检验的值

## 概述

判断传入值是否为文本。

## 示例

```excel
ISTEXT("1")
```

返回：  
TRUE

---

```excel
ISTEXT("")
```

返回：  
TRUE

---

```excel
ISTEXT(1)
```

返回：  
FALSE

---

```excel
ISTEXT(FALSE)
```

返回：  
FALSE
