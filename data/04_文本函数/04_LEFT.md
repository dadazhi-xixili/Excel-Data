# LEFT

## 语法

**LEFT**(文本[,长度=1])  
**LEFT**(text[,num_chars=1])

### 参数

1. 文本 text： 待提取的文本。
2. 长度 num_chars：要截取的文本长度。

## 概述

从文本开始位置截取指定长度文本。

### 补充

1. LEFTB 函数在未来的版本将弃用，请使用 LEFT 函数。

    - LEFTB 函数按字符节长度从文本开始位置截取指定长度文本。

    - 因即将弃用，不作补充。

## 示例

```excel
LEFT("Hello World",5)
```

返回：  
"Hello"

---

```excel
LEFT("Hello World",0)
```

返回：  
""

---

```excel
LEFT("Hello World")
```

返回：  
"H"
