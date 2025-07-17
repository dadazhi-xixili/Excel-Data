# VALUETOTEXT

## 语法

**VALUETOTEXT**(值[,模式=0])  
**VALUETOTEXT**(value[,format=0])

### 参数

1. 值 value：要转换的值。
2. 模式 format：转换模式。
    - 0：不转换文本。
    - 1：给文本添加双引号。

## 概述

将值转换为文本常量。

### 补充

1. 支持除数组外的类型，包括错误值。

## 示例

```excel
VALUETOTEXT(1)
```

返回：  
"1"

```excel
VALUETOTEXT("1",1)
```

返回：  
"""1"""

```excel
VALUETOTEXT(1/0)
```

返回：  
"#DIV/0!"
