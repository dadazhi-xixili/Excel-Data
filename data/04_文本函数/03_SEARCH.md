# SEARCH

## 语法

**SEARCH**(查找文本,文本,[开始位置])  
**SEARCH**(SEARCH_text,within_text[,start_num=1])

## 参数

1. 查找文本 SEARCH_text： 要查找的文本。
2. 文本 within_text： 待查找的文本。
3. 开始位置 start_num： 开始查找的位置。

## 概述

以不区分大小写方式查找文本在被查找文本第一次出现的位置。

### 补充

1. 可以使用通配符。
    - \* 匹配任意字符。
    - ? 匹配任意单个字符。
    - ~ 转义符。
1. SEARCHB 函数在未来的版本将弃用，请使用 SEARCH。
    - SEARCHB 函数返回文本中查找文本的起始位置。
    - 按字符节长度返回起始位置。
    - 因即将弃用，不作补充。
1. 未找到指定文本时，返回#VALUE!

## 示例

```excel
SEARCH("o", "Hello World")
```

返回：  
5

---

```excel
SEARCH("o", "Hello World", 6)
```

返回：  
8

---

```excel
SEARCH("o", "Hello World", 9)
```

返回：  
\#VALUE!

---

```excel
SEARCH("o?l", "Hello World")
```

返回：  
8
