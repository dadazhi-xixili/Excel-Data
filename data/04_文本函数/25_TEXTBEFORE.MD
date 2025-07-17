# TEXTBEFORE

## 语法

**TEXTBEFORE**(文本,分隔符[,分隔符索引=1,大小写=0,容错=0,错误替换=#N/A])  
**TEXTBEFORE**(text,delimiter,[instance_num=1,match_mode=0,match_end=0,if_not_found=#N/A])

### 参数

1. 文本 text：待处理的文本。
2. 分隔符 delimiter：分隔符。
3. 分隔符索引 instance_num：分隔符索引。
    - 正数：正序的分隔符索引。
    - 负数：倒序的分隔符索引。
4. 大小写 match_mode：
    - 0: 区分大小写。
    - 1: 不区分大小写。
5. 容错 match_end：
    - 0: 无匹配分隔符则返回错误替换(if_not_found)参数。
    - 1: 无匹配分隔符则返回文本本身。
6. 错误替换 if_not_found：错误替换。

## 概述

截取分隔符之前的文本。

### 补充

1. 分隔符可传入数组，且不会广播。

## 示例

### 常规

```excel
TEXTBEFORE("Hello World"," ")
```

返回：  
"Hello"

---

### 大小写示例

```excel
TEXTBEFORE("Hello World","w",,1)
```

返回：  
"Hello "

---

### 数组分隔符

```excek
TEXTBEFORE("Hello World",{"o"," "})
```

返回：  
"Hell"

---

### 分隔符索引

```excel
TEXTBEFORE("Hello World",{"o"," "},2)
```

返回：  
"Hello"

---

```excel
TEXTBEFORE("Hello World",{"o"," "},-1)
```

返回：  
"Hello W"

---

### 容错

```excel
TEXTBEFORE("Hello World","excel",,,1)
```

返回：  
"Hello World"

---

```excel
TEXTBEFORE("Hello World","excel",,,,"无")
```

返回：  
"无"
