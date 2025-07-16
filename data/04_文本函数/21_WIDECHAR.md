# WIDECHAR

## 语法

**WIDECHAR**(文本)  
**WIDECHAR**(text)

### 参数

1. 文本 text: 双字节(全角)文本。

## 概述

将单字节(半角)文本转换为对应的双字节(全角)文本。

### 补充

1. 双字节文本不会发生变化。

## 示例

```excel
WIDECHAR("ABC")
```

返回：  
"ＡＢＣ"
