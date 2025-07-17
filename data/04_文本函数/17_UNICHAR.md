# UNICHAR

## 语法

**UNICHAR**(数字)  
**UNICHAR**(number)

### 参数

1. 数字 number：字符编码。

## 概述

将字符编码转换为对应的字符。

### 补充

1. 支持的字符按 UNICODE 字符集。

## 示例

```excel
UNICHAR(65)
```

返回：  
"A"

---

```excel
UNICHAR(256)
```

返回：  
"Ā"

---

```excel
CHAR(256)
```

返回：  
#VALUE!
