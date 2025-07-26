# EXACT

## 语法

**EXACT**(文本\_1,文本\_2)  
**EXACT**(text1,text2)

## 概述

比较两个文本是否完全相同。

### 补充

1. (σ ｀ д′)σ 萝莉是笨蛋 💢💢💢
2. 文本直接`=`比较是忽略大小写的，EXACT 函数比较是区分大小写的。

## 示例

```excel
"Hello World" = "hello world"
```

返回：  
TRUE

---

```excel
EXACT("Hello World","hello world")
```

返回：  
FALSE
