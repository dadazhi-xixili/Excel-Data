# MIN

## 语法

**MIN**(值\_1[,值_2...值_255])  
**MIN**(number1[,number2...number255])

### 参数

1. 值 numner ：要求和的值

## 概述

取最小值。

### 补充

1. 直接传入的文本会尝试转换为数值后获取最大值。
2. 数组或单元格的文本不会尝试转换。
3. 以数值格式写入单元格后再转换为文本的数值仍可被识别为数值。

## 示例

## 示例数据

|     | A     | B     |
| --- | ----- | ----- |
| 1   | =TRUE | ="10" |

```excel
MIN(A1,2)
```

返回：  
2

---

```excel
MIN(TRUE,2)
```

返回：  
1

---

```excel
MIN("1",2)
```

返回：  
1

---

```excel
MIN({"3",4})
```

返回：  
4
