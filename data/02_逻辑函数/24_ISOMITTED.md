# ISOMITTED

## 语法

**ISOMITTED**(参数)  
**ISOMITTED**(argument)

### 参数

1. 参数 argument：LAMBDA 中的参数

## 概述

判断 LAMBDA 中的参数是否传入。

## 示例

```excel
LAMBDA(x,y,ISOMITTED(y))(1,)
```

返回：  
TRUE

---

```excel
LAMBDA(x,y,ISOMITTED(y))(1,)
```

返回：  
FALSE
