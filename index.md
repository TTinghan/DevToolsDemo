---
presentation:
theme: sky.css
  width: 800
  height: 600
  autoSlide: 0 
---
# Chrome DevTools 你还只会console.log么？

主讲： hantingting03
## 大纲：
-  常用调试技巧

-  快捷键的使用

## 常用调试技巧
#### 控制台中直接访问页面元素
- 先选中元素->再在控制台中使用$0查看元素
#### 访问最近选择的元素和对象
1. 控制台会存储最近 5 个被选择的元素和对象。当你在元素面板选择一个元素或在分析器面板选择一个对象,记录都会存储在栈中。
2. 可以使用$x来操作历史栈,x 是从 0 开始计数的,所以$0 表示最近选择的元素,$4 表示最后选择的元素。
#### 选择元素
1. $() - 返回满足指定 CSS 规则的第一个元素，此方法为 document.querySelector()的简化。
@import "devtools3.png"
2. $$() - 返回满足指定 CSS 规则的所有元素，此方法为 document.querySelectorAll()的简化。
@import "devtools4.png";
3. $x() - 返回满足指定 XPath 的所有元素。
@import "devtools5.png"
#### 访问最近的控制台结果
在控制台输入$_可以获控制台最近一次的输出结果。
@import "devtools1.png"
注意：
@import "devtools2.png"

#### console.table 代替 console.log
@import "devtools6.jpeg"

#### 使用 console.dir()/ dir() 代替 console.log
console.dir(object)/dir(object) 命令可以列出参数 object 的所有对象属性。
@import "devtools7.png"

#### 耗时监控
计时器：console.time(`String`) 和 console.timeEnd(`String`)
@import "devtools8.png"

#### 统计一个函数执行次数 console.count('打印了')
count()方法用于统计表达式被执行的次数,它接受一个字符串参数用于标记不同的记号。如果两次传入相同的字符串,该方法就会累积计数。
@import "devtools9.png"

## 全局键盘快捷键
#### 下列键盘快捷键可以在所有 DevTools 面板中使用:
@import "devtools10.png"

#### 控制台快捷键
@import "devtools11.png"

