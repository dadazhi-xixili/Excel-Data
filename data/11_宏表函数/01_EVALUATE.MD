# EVALUATE

## 语法

**EVALUATE**(表达式文本)  
**EVALUATE**(expression_text)

## 参数

1. 表达式文本 expression_text：文本组成的任意表达式。

## 概述

从文本中构建表达式，并计算结果。

## 示例

| Sheet1 | A   | B   | C   |
| ------ | --- | --- | --- |
| 1      | 1   | 2   | 3   |
| 2      | 4   | 5   | 6   |
| 3      | 7   | 8   | 9   |

```excel
EVA = LAMBDA(x,EVALUATE(x))
```

---

```excel
EVA("=SUM(A1:C1)")
```

返回：  
6

---

```excel
EVA("=LET(r,a1:c3,s,SUM(r),m,MAX(r),HSTACK(s,m))")
```

| 返回 |     |     |
| ---- | --- | --- |
|      | 45  | 9   |
