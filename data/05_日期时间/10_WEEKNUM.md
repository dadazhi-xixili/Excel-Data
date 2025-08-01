# WEEKNUM

## 语法

**WEEKNUM**(日期时间[,周类型=1])  
**WEEKNUM**(serial_number[,Return_type=1])

### 参数

1. 日期时间 serial_number：日期时间。
    - 文本值，则尝试转换。
    - 数值，则直接使用。
2. 周类型 Return_type：周类型。
    - 1：1 到 7 对应周日到周六。
    - 2：1 到 7 对应周一到周日。
    - 3：0 到 6 对应周一到周日。
    - 11：1 到 7 对应周一到周日。
    - 12：1 到 7 对应周二到周六。
    - 13：1 到 7 对应周三到周二。
    - 14：1 到 7 对应周四到周三。
    - 15：1 到 7 对应周五到周四。
    - 16：1 到 7 对应周六到周五。
    - 17：1 到 7 对应周日到周六。

## 概述

返回日期时间中的一年中的第几周。

## 示例

```excel
WEEKNUM(45859.2178209491)
WEEKNUM("45859.2178209491")
WEEKNUM(2025/07/21 05:13:40)
WEEKNUM("2025/07/21 05:13:40")
```

返回：  
30
