# FILES

## 语法

**FILES**(文件路径)  
**FILES**(path)

## 参数

1. 文件路径 path：文件路径。
    - 支持通配符

## 概述

从文件夹路径中获取文件名称数组。

### 补充

1. 只能是文件噢，不包括文件夹中的文件夹。

## 示例

```excel
GetFiles = LAMBDA(x,TOCOL(FILES(x)))
GetFiles("C:\Excel_Toolkit\Excel Toolkit\excel?tool*")
```

| 返回 |                    |
| ---- | ------------------ |
|      | Excel_Toolkit.css  |
|      | Excel_Toolkit.db   |
|      | Excel_Toolkit.exe  |
|      | Excel_Toolkit.html |
|      | Excel_Toolkit.js   |
