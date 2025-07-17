# ISEVEN

## 语法

**ISEVEN**(值)  
**ISEVEN**(value)

### 参数

1. 值 value ：检验的值。

## 概述

判断传入值是否为偶数。

### 补充

1. 传入单元格区域时应先转换为数组，否则报错。

## 示例

```excel
ISEVEN(1)
```

返回：  
FALSE

---

```excel
ISEVEN(2)
```

返回：  
TRUE

---

```excel
ISEVEN(4.1)
```

返回：  
TRUE

---

```excel
ISEVEN("")
```

返回：  
FALSE

---

```excel
ISEVEN(FALSE)
```

返回：  
FALSE
