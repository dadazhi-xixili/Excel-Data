# SUBSTITUTE

## 语法

**SUBSTITUTE**(文本,旧文本,替换文本[,第几个旧文本])  
**SUBSTITUTE**(text,old_text,new_text[,instance_num])

### 参数

1. 文本 text：要进行替换的文本。
2. 旧文本 old_text：被替换的文本。
3. 替换文本 new_text：替换文本。
4. 替换次数 instance_num：替换的次数。

## 概述

使用新文本替换文本中的旧文本。

### 补充

1. 省略 instance_num 参数时，默认替换所有匹配项。

## 示例

```excel
SUBSTITUTE("Hello World", "World", "Excel")
```

返回：  
"Hello Excel"

---

```excel
SUBSTITUTE("111111", "1", "2", 3)
```

返回：  
"112111"
