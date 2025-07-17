# UNICODE

## 语法

**UNICODE**(文本)  
**UNICODE**(text)

### 参数

1. 文本 text：待处理的文本。

## 概述

获取文本首字符的 UNICODE 编码。

## 示例

## 示例

```excel
UNICODE("A")
```

返回：  
65

---

```excel
// UNICHAR(256) = "Ā"
CODE(UNICHAR(256))
```

返回：  
63

---

```excel
// UNICHAR(256) = "Ā"
UNICODE(UNICHAR(256))
```

返回：  
256
