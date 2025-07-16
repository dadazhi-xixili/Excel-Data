# REPLACE

## 语法

**REPLACE**(文本,开始位置,长度,替换文本)  
**REPLACE**(old_text,start_num,num_chars,new_text)

### 参数

1. 文本 old_text：待替换的文本。
2. 开始位置 start_num：替换的起始位置。
3. 长度 num_chars：要替换的文本长度。
4. 替换文本 new_text：替换的文本。

## 概述

从指定位置替换指定长度的文本。

### 补充

1. REPLACEB 函数在未来的版本将弃用，请使用 REPLACE 函数。
    - REPLACEB 函数指定位置替换指定长度的文本,位置长度均按字符节长度。
    - 因即将弃用，不作补充。

## 示例

```excel
REPLACE("Hello World",1,5,"Hi")
```

输出：  
"Hi World"

```excel
REPLACE("114514",3,2,"💥💥")
```

输出：  
"11💥💥14"
