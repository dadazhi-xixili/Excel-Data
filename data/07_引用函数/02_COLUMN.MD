# COLUMN

## 语法

**COLUMN**([单元格])  
**COLUMN**([reference])

### 参数

1. 区域 reference：单元格
    - 省略则为公式所在单元格

## 概述

返回引用区域的列号。

### 补充

1. 传入多行不会增加返回列数。
2. 传入多列会返回单行数组。

## 示例

```excel
COLUMN(B1)
```

返回：  
2

---

```excel
COLUMN(B2:C3)
```

| 返回 |     |     |
| ---- | --- | --- |
|      | 2   | 3   |

---

```excel
COLUMN(A2:B3)
```

| 返回 |     |     |
| ---- | --- | --- |
|      | 1   | 2   |

---

```excel
COLUMN(C:C)
```

返回：  
3
