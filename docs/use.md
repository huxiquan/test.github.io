### Selenium IDE常用命令
#### add selection
将选择添加到多选元素中的选项集.  
```参数：```  
locator：元素定位器。value：要输入的值。
#### answer on next prompt
影响下一个警报提示。此命令将向其发送指定的答案字符串。如果警报已经存在，请改用“可见提示时的webdriver回答”.  
```参数：```  
answer：提示弹出窗口时给出的答案
#### assert  
检查变量是否为期望值。变量的值将转换为字符串以进行比较。如果断言失败，则测试将停止.  
```参数```  
variable name(变量名)：不带括号的变量名.  
expected value(期望值):您期望变量包含的结果（例如，true，false或其他某个值）
#### assert alert  
确认已使用提供的文本呈现警报。如果断言失败，则测试将停止  
```参数```  
alert text(提示内容): 要检查的内容  
#### assert checked
确认目标元素已被检查。如果断言失败，则测试将停止。  
```参数```  
locator：元素定位器  
#### assert confirmation  
确认已提交确认。如果断言失败，则测试将停止。  
```参数```  
text：要使用的文本  
#### assert editable
确认目标元素是可编辑的。如果断言失败，则测试将停止。  
```参数```  
locator：元素定位器。  
#### assert element present
确认目标元素存在于页面上的某处。如果断言失败，则测试将停止。  
```参数```  
locator：元素定位器。  
#### assert element not present
确认目标元素不在页面上任何地方。如果断言失败，则测试将停止。  
```参数```  
locator：元素定位器。
#### assert not checked
确认尚未检查目标元素。如果断言失败，则测试将停止。  
```参数```  
locator：元素定位器
#### assert not editable
确认目标元素不可编辑。如果断言失败，则测试将停止  
```参数```  
locator：元素定位器
#### assert not selected value
确认下拉元素中所选选项的value属性不包含提供的值。如果断言失败，则测试将停止。  
```参数```  
select locator：标识下拉菜单的元素定位器.  
text：完全匹配的字符串。正在支持模式匹配。有关详细信息，请参见https://github.com/SeleniumHQ/selenium-ide/issues/141。  
#### assert not text
确认元素的文本不包含提供的值。如果断言失败，则测试将停止。  
```参数```  
locator：元素定位器.  
text：完全匹配的字符串。正在支持模式匹配。有关详细信息，请参见https://github.com/SeleniumHQ/selenium-ide/issues/141。

#### assert prompt
确认已呈现JavaScript提示。如果断言失败，则测试将停止。  
```参数```  
text：要使用的文本  
#### assert selected value
确认下拉元素中所选选项的value属性包含提供的值。如果断言失败，则测试将停止。  
```参数```  
select locator：标识下拉菜单的元素定位器.  
text：完全匹配的字符串。正在支持模式匹配。有关详细信息，请参见https://github.com/SeleniumHQ/selenium-ide/issues/141。

#### assert selected label
确认下拉菜单中所选选项的标签包含提供的值。如果断言失败，则测试将停止。  
```参数```  
select locator：标识下拉菜单的元素定位器.  
text：完全匹配的字符串。正在支持模式匹配。有关详细信息，请参见https://github.com/SeleniumHQ/selenium-ide/issues/141。  
#### assert text
确认元素的文本包含提供的值。如果断言失败，则测试将停止。  
```参数```  
select locator：标识下拉菜单的元素定位器.  
text：完全匹配的字符串。正在支持模式匹配。有关详细信息，请参见https://github.com/SeleniumHQ/selenium-ide/issues/141。。
#### assert title
确认当前页面的标题包含提供的文本。如果断言失败，则测试将停止。  
```参数```  
text：完全匹配的字符串。正在支持模式匹配。有关详细信息，请参见https://github.com/SeleniumHQ/selenium-ide/issues/141。  
#### assert value
确认输入字段的（空白修饰）值（或其他带有value参数的值）。对于复选框/无线电元素，根据是否选中该元素，其值为“ on”或“ off”。如果断言失败，则测试将停止。  
```参数```  
locator：元素定位器。  
text：完全匹配的字符串。正在支持模式匹配。有关详细信息，请参见https://github.com/SeleniumHQ/selenium-ide/issues/141。

#### check
检查一个切换按钮（复选框/单选）。  
```参数```  
locator：元素定位器
#### choose cancel on next confirmation
影响下一个确认警报。此命令将取消它。如果警报已经存在，则使用“ webdriver选择在可见确认时取消”。
#### choose cancel on next prompt
影响下一个警报提示。此命令将取消它。如果警报已经存在，则使用“ webdriver在可见的提示下选择取消”。
#### choose ok on next confirmation
影响下一个确认警报。此命令将接受它。如果警报已经存在，则使用“ Webdriver在可见确认中选择确定”。
#### click
单击目标元素（例如，链接，按钮，复选框或单选按钮）。  
```参数```  
locator：元素定位器。

#### click at
单击目标元素（例如，链接，按钮，复选框或单选按钮）。坐标相对于目标元素（例如，0,0是元素的左上角），并且主要用于检查在其上传递的效果，例如材料波纹效果。  
```参数```  
locator：元素定位器,  
坐标字符串：指定鼠标事件相对于从定位器找到的元素的x，y位置（例如-10,20）  
#### close
关闭当前窗口。无需关闭初始窗口，IDE会重新使用它；关闭它可能会导致测试性能下降。
#### debugger
中断执行并进入调试器
#### do
创建一个至少执行一次执行命令的循环。使用repeat if命令终止分支。
#### double click
双击元素（例如，链接，按钮，复选框或单选按钮）。  
```参数```  
locator：元素定位器。  
#### drag and drop to object
拖动一个元素并将其拖放到另一个元素上.  
```参数```  
要拖动的对象的定位器：要拖动的元素的定位器.  
拖动目标对象的定位器：放置元素（其位置（例如，其中的最中心像素）将成为要拖动的对象的定位器）的点的定位器。
#### echo
将指定的消息打印到Selenese表中的第三个表单元格中。对于调试很有用.  
```参数```  
message：要打印的消息。
#### edit content
设置内容可编辑元素的值，就像您在其中键入一样  
```参数```  
locator：元素定位器.  
value：要输入的值。
#### else
if块的一部分。如果不满足if和/或else if条件，请在此分支中执行命令。使用end命令终止分支。

#### else if
if块的一部分。如果不满足if条件，请在此分支中执行命令。使用end命令终止分支.  
```参数```  
条件表达式：JavaScript表达式，它返回布尔值以用于控制流命令。
#### end
终止控制流块是否为时，为时和为时间。
#### execute script
在当前选定的框架或窗口的上下文中执行一段JavaScript。脚本片段将作为匿名函数的主体执行。要存储返回值，请使用“ return”关键字，并在值输入字段中提供变量名称。  
```参数```  
script：要运行的JavaScript代码段.  
变量名：不带括号的变量名。
#### execute async script
在当前选定的框架或窗口的上下文中执行JavaScript的异步代码段。脚本片段将作为匿名函数的主体执行，并且必须返回Promise。如果您使用'return'关键字，则Promise结果将保存在变量中。  
```参数```  
script：要运行的JavaScript代码段.  
变量名：不带括号的变量名。

#### for each
创建一个循环，为给定集合中的每个项目执行执行命令。  
```参数```  
数组变量名称：包含JavaScript数组的变量的名称。  
迭代器变量名称：在循环控制流命令中迭代集合时（例如，针对每个变量）使用的变量名称。
#### if
在测试中创建条件分支。使用end命令终止分支。  
```参数```  
条件表达式：JavaScript表达式，它返回布尔值以用于控制流命令。
#### mouse down
模拟用户按下鼠标左键（尚未释放它）。  
```参数```  
locator：元素定位器。
#### mouse down at
模拟用户在指定位置按下鼠标左键（尚未释放它）。  
```参数```  
locator：元素定位器.  
坐标字符串：指定鼠标事件相对于从定位器找到的元素的x，y位置（例如-10,20）。


#### mouse move at
模拟用户在指定元素上按下鼠标按钮（尚未释放它）.  
```参数```  
locator：元素定位器.  
坐标字符串：指定鼠标事件相对于从定位器找到的元素的x，y位置（例如-10,20）。



