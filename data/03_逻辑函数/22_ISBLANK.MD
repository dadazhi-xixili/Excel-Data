# ISBLANK
## 语法

**ISBLANK**(引用)  
**ISBLANK**(reference)

### 参数

1. 引用 reference ：检验的值

## 概述

判断传入值是否为引用空白单元格。

## 示例

## 示例数据

|     | A   | B   | C    |
| --- | --- | --- | ---- |
| 1   | 1   | "A" | NA() |
| 2   |
| 3   |

```
ISBLANK(A1)
输出：
FALSE

ISBLANK(A2)
输出：
TRUE

ISBLANK("")
输出：
FALSE

ISBLANK(1)
输出：
FALSE

ISBLANK(TRUE)
输出：
FALSE

ISBLANK(A1:C3)
```

| 输出 |       |       |       |
| ---- | ----- | ----- | ----- |
|      | FALSE | FALSE | FALSE |
|      | TRUE  | TRUE  | TRUE  |
|      | TRUE  | TRUE  | TRUE  |
