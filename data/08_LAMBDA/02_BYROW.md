# BYROW

## 语法

**BYROW**(数组,自定义函数(行,表达式) | 函数)  
**BYROW**(array,LAMBDA(row,calculation) | function)

### 参数

1. 数组 array：要处理的数组。
2. 自定义函数 LAMBDA：处理数组的函数。
3. 函数 function：处理数组的函数。
4. 行 row：当前处理的行，名称可以自定义。

## 概述

数组中的每一行执行传入的函数。

### 常见错误

1. 传入的函数返回必须是一个值，不能是数组，否则因无法展开报错。

## 示例

### 示例源

|     | A   | B   | C   |
| --- | --- | --- | --- |
| 1   | 1   | 2   | 3   |
| 2   | 4   | 5   | 6   |
| 3   | 7   | 8   | 9   |

#### 传入自定义函数

```excel
BYROW(A1:C3,LAMBDA(row,SUM(row)*2))
```

|     | A   | B   | C   | 过程            | 返回 |
| --- | --- | --- | --- | --------------- | ---- |
| 1   | 1   | 2   | 3   | SUM({1,2,3})\*2 | 12   |
| 2   | 4   | 5   | 6   | SUM({4,5,6})\*2 | 30   |
| 3   | 7   | 8   | 9   | SUM({7,8,9})\*2 | 48   |

---

#### 传入函数

```excel
BYROW(A1:C3,SUM)
```

|     | A   | B   | C   | 过程         | 返回 |
| --- | --- | --- | --- | ------------ | ---- |
| 1   | 1   | 2   | 3   | SUM({1,2,3}) | 6    |
| 2   | 4   | 5   | 6   | SUM({4,5,6}) | 15   |
| 3   | 7   | 8   | 9   | SUM({7,8,9}) | 24   |
