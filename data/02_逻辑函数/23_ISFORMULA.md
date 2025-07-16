# ISFORMULA

## 语法

**ISFORMULA**(引用)  
**ISFORMULA**(reference)

### 参数

1. 引用 value ：检验的引用。

## 概述

判断传入值是否为引用公式单元格。

## 示例

## 示例数据

|     | A   | B    | C     |
| --- | --- | ---- | ----- |
| 1   | 1   | "A"  |       |
| 2   | =1  | =1/0 | =PI() |
| 3   |

```
ISFORMULA(A1)
输出：
FALSE

ISFORMULA(A2)
输出：
TRUE

ISFORMULA("")
输出：
FALSE

ISFORMULA(1)
输出：
FALSE

ISFORMULA(TRUE)
输出：
FALSE

ISFORMULA(A1:C3)
```

| 输出 |       |       |       |
| ---- | ----- | ----- | ----- |
|      | FALSE | FALSE | FALSE |
|      | TRUE  | TRUE  | TRUE  |
|      | FALSE | FALSE | FALSE |
