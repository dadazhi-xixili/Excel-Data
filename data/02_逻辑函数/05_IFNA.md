# IFNA

## 语法

**IFNA**(值,值不可用返回值)  
**IFNA**(value,value_if_na)

### 参数

1. 值 value：要检查的值。
2. 值不可用返回值 value_if_na：如果值为#N/A，则返回该值。

## 概述

值参数如果捕获#N/A 错误值，则返回指定值。

## 补充

1. value_if_na 默认为 0，但","必须输入。
2. 只能用于处理#N/A 错误值，其他错误值会返回错误值。

## 示例

```excel
IFNA(NA(),"遇到了NA")
```

过程：  
IFNA(#N/A,"遇到了 NA")  
输出：  
"遇到了 NA"

---

```excel
IFNA(1/0,"遇到了错误")
```

过程：  
IFNA(#DIV/0!,0)  
输出：  
#DIV/0!
