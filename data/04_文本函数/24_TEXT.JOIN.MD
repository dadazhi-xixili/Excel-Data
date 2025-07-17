# TEXTJOIN

## 语法

**TEXTJOIN**(分隔符,忽略空值=TRUE,文本\_1[,文本_2...文本_252])  
**TEXTJOIN**(delimiter,ignore_empty,text1[,text2...,text252])

### 参数

1. 分隔符 delimiter：文本之间的分隔符。
2. 忽略空值 ignore_empty：
    - TRUE：忽略空值。
    - FALSE：不忽略空值。
3. 文本 text：待拼接的文本。

## 概述

使用分隔符连接多个文本。

### 补充

1. 分隔符可传递数组，按数组中的字符出现顺序循环插入连接。

## 示例

### 常规示例

```excel
TEXTJOIN(",",0,"1","2","3")
```

返回：  
"A,,B,C"

```excel
TEXTJOIN(",",,{"A","";"B","C"})
```

返回：  
"A,B,C"

### 数组分隔符

```excel
TEXTJOIN({",",";"},,{1,2,3,4,5,6,7,8})
```

返回：  
"1,2;3,4;5,6;7,8"
