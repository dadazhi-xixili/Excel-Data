# ADDRESS

## 语法

**ADDRESS**(行号,列号[,引用类型=1,a1=TRUE,工作表名])  
**ADDRESS**(row_num,column_num,[abs_num=1,a1=TRUE,sheet_text])

### 参数

1. 行号 row_num：行号。
2. 列号 column_num：列号。
3. 引用类型 abs_num：引用类型。
    - 1：绝对引用。
    - 2：绝对引用行。
    - 3：绝对引用列。
    - 4：相对引用。
4. a1 : 引用模式。
    - TRUE：返回 A1 引用。
    - FALSE：返回 R1C1 引用。
5. 工作表名 sheet_text：工作表名称。
    - 其实就是个自定义前缀，把工作簿名写上都行。

## 示例

```excel
ADDRESS(1,2)
```

返回：  
"$A$2"

---

```excel
ADDRESS(1,2,2)
```

返回：  
"A$2"

---

```excel
ADDRESS(1,2,3)
```

返回：  
"$A2"

---

```excel
ADDRESS(1,2,4)
```

返回：  
"A2"

---

```excel
ADDRESS(1,2,1,FALSE)
```

返回：  
"R1C2"

---

```excel
ADDRESS(1,2,4,1,"[萝莉是笨蛋.xlsx]'第九百九十九种笨法'!")
```

返回：  
"[萝莉是笨蛋.xlsx]'第九百九十九种笨法'!A2"
