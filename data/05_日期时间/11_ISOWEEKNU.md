# ISOWEEKNU

## 语法

**ISOWEEKNUM**(日期)  
**ISOWEEKNUM**(date)

### 参数

1. 日期时间 serial_number：日期时间。
    - 文本值，则尝试转换。
    - 数值，则直接使用。

## 概述

以 ISO 标准返回日期时间中的一年中的第几周。

### 补充

1. ISO 标准周计算规则：
    - 周一为星期开始。
    - 包含第一个周四的周为一年中的第一周。

## 示例

```excel
ISOWEEKNUM("2023/01/01")
```

返回：  
52

---

```excel
WEEKNUM("2023/01/01")
```

返回：  
1
