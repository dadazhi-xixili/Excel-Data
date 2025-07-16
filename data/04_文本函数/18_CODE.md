# CODE

## 语法

**CODE**(文本)  
**CODE**(text)

### 参数

1. 文本 text：待处理的文本。

## 概述

获取文本首字符的编码。

### 补充

1. 支持的字符根据 EXCEL 所在系统环境确定。
2. 不支持的字符可能会出现意料外的编码。

## 示例

```excel
CODE("A")
```

返回：  
65

```excel
// UNICHAR(256) = "Ā"
CODE(UNICHAR(256))
```

返回：  
63

```excel
// UNICHAR(256) = "Ā"
UNICODE(UNICHAR(256))
```

返回：  
256
