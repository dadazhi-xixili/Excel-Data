# MATCH

## 语法

**MATCH**(查找值,查找数组[,匹配模式=1])  
**MATCH**(lookup_value,lookup_array[,match_type=1])

### 参数

1. 查找值 lookup_value：查找值。
2. 查找数组 lookup_array：要查找的数组或区域。
3. 匹配模式 match_type：匹配模式。
    - 0：精确查找值，线性匹配模式。
    - -1：小于等于查找值，二分法匹配模式。
    - 1：大于等于查找值，二分法匹配模式。

## 概述

第一个匹配值所在索引。

### 补充

1. 二分法匹配逻辑可以参考同时启用了第 5 参(match_mode)和第 6 参(search_mode)XLOOKUP 函数。
2. 我真的不是不想 ✍ 写示例 ¯\\\_(ツ)\_/¯

## 示例

### 示例数据

|     | A   | B   |
| --- | --- | --- |
| 1   | 10  | M   |
| 2   | 20  | L   |
| 3   | 30  | K   |
| 4   | 40  | J   |
| 5   | 50  | I   |
| 6   | 60  | H   |
| 7   | 70  | G   |
| 8   | 80  | F   |
| 9   | 90  | E   |
| 10  | 100 | D   |
| 11  | 110 | C   |
| 12  | 120 | B   |
| 13  | 130 | A   |

### 常规

```excel
XMATCH(80,A1:A13,)
```

返回：  
8

---

### 二分法大于等于

```excel
XMATCH(85,A1:A13,1)
```

返回：  
9

### 二分法小于等于

```excel
XMATCH(85,A1:A13,-1)
```

返回：  
8
