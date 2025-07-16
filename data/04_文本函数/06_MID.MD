## MID

## 语法

**MID**(文本,开始位置,长度)  
**MID**(text,start_num,num_chars)

### 参数

1. 文本 text： 待提取的文本。
2. 开始位置 start_num： 提取的起始位置。
3. 长度 num_chars： 提取的文本长度。

## 概述

从指定开始位置截取指定长度文本。

### 补充

1. MIDB 函数在未来的版本将弃用，请使用 MID 函数。

    - MIDB 函数按按字符节长度从指定开始位置截取指定长度文本。
    - 因即将弃用，不作补充。

2. 开始位置小于 1 或长度小于 0 则返回#VALUE!。
3. 开始位置大于文本长度或长度为 0 值则返回""。

## 示例

```excel
MID("Hello World",1,5)
```

返回：  
"Hello"

```excel
MID("Hello World",1,0)
```

返回：  
""

```excel
MID("Hello World",1,100)
```

返回：  
"Hello World"

```excel
MID("Hello World",6,5)
```

返回：  
"World"
