# SWITCH
## 语法
**SWITCH**(匹配值,匹配项1,返回值1[,匹配项2,返回值2,...匹配项126,返回值126,默认值])      
**SWITCH**(expression,value1,result1[,value2,result2,...value126,result126,default])
### 参数
1. 匹配值 expression：要匹配的值。
2. 匹配项 value: 与匹配值进行比较的值。
3. 返回值 result：如果匹配项的值等于匹配值，则返回该值。
4. 默认值 default：如果匹配项的值都不等于匹配值，则返回该值。
## 概述
返回匹配值的对应的匹配项。
### 补充
1. 与IF和IFS函数不同，匹配项如果传入表达式，会先进行运算。
## 常见错误
1. 匹配项与返回值应该成对输入，否则报错。
2. 当省略默认值且无对应匹配项是，返回#N/A。
## 示例
```excel
A1 = 60
SWITCH(TRUE,A1>=90,"A",A1>=80,"B",A1>=70,"C",A1>=60,"D","E")
过程：
SWITCH(TRUE,FALSE,"A",FALSE,"B",FALSE,"C",TRUE,"D","E")
SWITCH(TRUE,FALSE,"B",FALSE,"C",TRUE,"D","E")
SWITCH(TRUE,FALSE,"C",TRUE,"D","E")
SWITCH(TRUE,TRUE,"D","E")
输出：
"D"
```
```excel
SWITCH(2,1,"周日",2, "周一",3, "周二",4, "周三",5, "周四",
6, "周五",7, "周六","无效日期")
输出：
"周一"

SWITCH(8,1,"周日",2, "周一",3, "周二",4, "周三",5, "周四",
6, "周五",7, "周六","无效日期")
输出：
"无效日期”

SWITCH(8,1,"周日",2, "周一",3, "周二",4, "周三",5, "周四",
6, "周五",7, "周六")
输出：
#N/A
```
