# CHOOSECOLS

## 语法

**CHOOSECOLS**(数组,列号 1,[列号 2],…)  
**CHOOSECOLS**(array,col_num1,[col_num2],…)

### 参数

1. 数组 array：引用的数组。
2. 列号 col_num：要返回的列的编号。

## 概述

从数组中选择指定列。

### 补充

1. 多列选择会横向拼接。

## 示例

### 示例数据

|     | A   | B   | C   | D   |
| --- | --- | --- | --- | --- |
| 1   | 1   | 2   | 3   | 4   |
| 2   | 5   | 6   | 7   | 8   |
| 3   | 9   | 10  | 11  | 12  |
| 4   | 13  | 14  | 15  | 16  |

```excel
CHOOSECOLS(A1:D4,2)
```

| 返回 |     |
| ---- | --- |
|      | 4   |
|      | 8   |
|      | 12  |
|      | 16  |

---

```excel
CHOOSECOLS(A1:D4,1,3)
```

| 返回 |     |     |
| ---- | --- | --- |
|      | 1   | 3   |
|      | 5   | 7   |
|      | 9   | 11  |
|      | 13  | 15  |
