# FIND

## 语法

**FIND**(查找文本,文本,[开始位置])  
**FIND**(find_text,within_text[,start_num=1])

## 参数

1. 查找文本 find_text： 要查找的文本。
2. 文本 within_text： 待查找的文本。
3. 开始位置 start_num： 开始查找的位置。

## 概述

查找文本在被查找文本第一次出现的位置。

### 补充

1. FINDB 函数在未来的版本将弃用，请使用 FIND。
    - FINDB 函数返回文本中查找文本的起始位置。
    - 按字符节长度返回起始位置。
    - 因即将弃用，不作补充。
2. 未找到指定文本时，返回#VALUE!

## 示例

```excel
FIND("o", "Hello World")
```

返回：  
5

---

```excel
FIND("o", "Hello World", 6)
```

返回：  
8

---

```excel
FIND("o", "Hello World", 9)
```

返回：  
\#VALUE!
