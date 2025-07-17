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

```excel
ISFORMULA(A1)
```

返回：  
FALSE

---

```excel
ISFORMULA(A2)
```

返回：  
TRUE

---

```excel
ISFORMULA("")
```

返回：  
FALSE

---

```excel
ISFORMULA(1)
```

返回：  
FALSE

---

```excel
ISFORMULA(TRUE)
```

返回：  
FALSE

---

```excel
ISFORMULA(A1:C3)
```

| 返回 |       |       |       |
| ---- | ----- | ----- | ----- |
|      | FALSE | FALSE | FALSE |
|      | TRUE  | TRUE  | TRUE  |
|      | FALSE | FALSE | FALSE |
