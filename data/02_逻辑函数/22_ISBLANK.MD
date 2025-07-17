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

```excel
ISBLANK(A1)
```

返回：  
FALSE

---

```excel
ISBLANK(A2)
```

返回：  
TRUE

---

```excel
ISBLANK("")
```

返回：  
FALSE

---

```excel
ISBLANK(1)
```

返回：  
FALSE

---

```excel
ISBLANK(TRUE)
```

返回：  
FALSE

---

```excel
ISBLANK(A1:C3)
```

| 返回 |       |       |       |
| ---- | ----- | ----- | ----- |
|      | FALSE | FALSE | FALSE |
|      | TRUE  | TRUE  | TRUE  |
|      | TRUE  | TRUE  | TRUE  |
