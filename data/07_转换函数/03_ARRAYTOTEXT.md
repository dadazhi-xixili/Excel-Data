# ARRAYTOTEXT

## 语法

**ARRAYTOTEXT**(数组[,模式=0])  
**ARRAYTOTEXT**(array[,format=0])

### 参数

1. 数组 array：要转换的数组。
2. 模式 format：
    - 0：以值在单元格中的样式合并。
    - 1：以可解析的数组表达式形式返回。

## 概述

将数组转换为文本。

## 示例

```excel
ARRAYTOTEXT({#N/A,2;"A",2})
```

返回：  
"#N/A, 2, A, 2"

```excel
ARRAYTOTEXT({#N/A,2;"A",2},1)
```

返回：  
"{#N/A,2;""A"",2}"
