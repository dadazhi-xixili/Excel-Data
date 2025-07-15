# IFERROR
## 语法
**IFERROR**(值,错误返回值)          
**IFERROR**(value,value_if_error)
### 参数
1. 值 value：要检查的值。
2. 错误返回值 value_if_error：如果值包含错误，则返回该值。
## 概述
值参数如果捕获任何错误值，则返回指定值。
## 补充
1. value_if_error默认为0，但","必须输入。
## 示例
```excel
IFERROR(1/0,)
过程：
IFERROR(#DIV/0!,0)
输出：
0
```