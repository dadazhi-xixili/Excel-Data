# COUNTBLANK

## 语法

**COUNTBLANK**(单元格集合)  
**COUNTBLANK**(range)

### 参数

1. 单元格集合 range：要统计的单元格。

## 概述

统计空值。

## 示例

|     | A     | B     |
| --- | ----- | ----- |
| 1   | ="A"  | =1    |
| 2   | =NA() | =TRUE |
| 3   | =""   |       |

```excel
COUNTBLANK(A1:B3)
```

输出：  
2
