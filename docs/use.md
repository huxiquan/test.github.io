### AutoTCG专业版常用命令
#### add selection
将选择添加到多选元素中的选项集.  
##### 参数 
* locator：元素定位器  
* value：要输入的值  

#### answer on next prompt
影响下一个警报提示。此命令将向其发送指定的答案字符串。如果警报已经存在，请改用“可见提示时的webdriver回答”.   
##### 参数
* answer：提示弹出窗口时给出的答案  

#### assert 
检查变量是否为期望值。变量的值将转换为字符串以进行比较。如果断言失败，则测试将停止.  
##### 参数
* variable name(变量名)：不带括号的变量名.  
* expected value(期望值):您期望变量包含的结果（例如，true，false或其他某个值）  

#### assert alert
确认已使用提供的文本呈现警报。如果断言失败，则测试将停止  
##### 参数
* alert text(提示内容): 要检查的内容  

#### assert checked
确认目标元素已被检查。如果断言失败，则测试将停止。  
##### 参数
* locator：元素定位器  

#### assert confirmation
确认已提交确认。如果断言失败，则测试将停止。  
##### 参数
* text：要使用的文本  

#### assert editable
确认目标元素是可编辑的。如果断言失败，则测试将停止。  
##### 参数
* locator：元素定位器  

#### assert element present
确认目标元素存在于页面上的某处。如果断言失败，则测试将停止  
##### 参数 
* locator：元素定位器  

#### assert element not present
确认目标元素不在页面上任何地方。如果断言失败，则测试将停止  
##### 参数  
* locator：元素定位器  

#### assert not checked
确认尚未检查目标元素。如果断言失败，则测试将停止。  
##### 参数
* locator：元素定位器  

#### assert not editable
确认目标元素不可编辑。如果断言失败，则测试将停止  
##### 参数  
* locator：元素定位器  

#### assert not selected value
确认下拉元素中所选选项的value属性不包含提供的值。如果断言失败，则测试将停止  
##### 参数  
* select locator：标识下拉菜单的元素定位器.  
* text：完全匹配的字符串。正在支持模式匹配。有关详细信息，请参见[链接](https://github.com/SeleniumHQ/selenium-ide/issues/141)  

#### assert not text
确认元素的文本不包含提供的值。如果断言失败，则测试将停止  
##### 参数  
* locator：元素定位器.  
* text：完全匹配的字符串。正在支持模式匹配。有关详细信息，请参见 [链接](https://github.com/SeleniumHQ/selenium-ide/issues/141)  

#### assert prompt
确认已呈现JavaScript提示。如果断言失败，则测试将停止  
##### 参数
* text：要使用的文本  

#### assert selected value
确认下拉元素中所选选项的value属性包含提供的值。如果断言失败，则测试将停止  
##### 参数  
* select locator：标识下拉菜单的元素定位器.  
* text：完全匹配的字符串。正在支持模式匹配。有关详细信息，请参见[链接](https://github.com/SeleniumHQ/selenium-ide/issues/141)  

#### assert selected label
确认下拉菜单中所选选项的标签包含提供的值。如果断言失败，则测试将停止  
##### 参数  
* select locator：标识下拉菜单的元素定位器.  
* text：完全匹配的字符串。正在支持模式匹配。有关详细信息，请参见[链接](https://github.com/SeleniumHQ/selenium-ide/issues/141)  

#### assert text
确认元素的文本包含提供的值。如果断言失败，则测试将停止  
##### 参数  
* select locator：标识下拉菜单的元素定位器.  
* text：完全匹配的字符串。正在支持模式匹配。有关详细信息，请参见[链接](https://github.com/SeleniumHQ/selenium-ide/issues/141)  

#### assert title
确认当前页面的标题包含提供的文本。如果断言失败，则测试将停止  
##### 参数  
* text：完全匹配的字符串。正在支持模式匹配。有关详细信息，请参见[链接](https://github.com/SeleniumHQ/selenium-ide/issues/141)  

#### assert value
确认输入字段的（空白修饰）值（或其他带有value参数的值）。对于复选框/单选元素，根据是否选中该元素，其值为“ on”或“ off”。如果断言失败，则测试将停止  
##### 参数  
* locator：元素定位器。  
* text：完全匹配的字符串。正在支持模式匹配。有关详细信息，请参见[链接](https://github.com/SeleniumHQ/selenium-ide/issues/141)  

#### check
检查一个切换按钮（复选框/单选）。  
##### 参数
* locator：元素定位器  

#### choose cancel on next confirmation
影响下一个确认警报。此命令将取消它。如果警报已经存在，则使用“ webdriver选择在可见确认时取消”  

#### choose cancel on next prompt
影响下一个警报提示。此命令将取消它。如果警报已经存在，则使用“ webdriver在可见的提示下选择取消”。  

#### choose ok on next confirmation
影响下一个确认警报。此命令将接受它。如果警报已经存在，则使用“ Webdriver在可见确认中选择确定”。  

#### click
单击目标元素（例如，链接，按钮，复选框或单选按钮）  
##### 参数
* locator：元素定位器。  

#### click at
单击目标元素（例如，链接，按钮，复选框或单选按钮）。坐标相对于目标元素（例如，0,0是元素的左上角），并且主要用于检查在其上传递的效果，例如材料波纹效果  
##### 参数  
* locator：元素定位器  
* 坐标字符串：指定鼠标事件相对于从定位器找到的元素的x，y位置（例如-10,20）  
#### click right
用鼠标右键点击目标元素（例如，链接，按钮，复选框或单选按钮）
##### 参数
* locator：元素定位器 
#### close
关闭当前窗口。无需关闭初始窗口，IDE会重新使用它；关闭它可能会导致测试性能下降  

#### debugger
中断执行并进入调试器  

#### do
创建一个至少执行一次执行命令的循环。使用repeat if命令终止分支  

#### double click
双击元素(例如，链接，按钮，复选框或单选按钮)  
##### 参数
* locator：元素定位器  

#### drag and drop to object
拖动一个元素并将其拖放到另一个元素上.  
##### 参数  
* 要拖动的对象的定位器：要拖动的元素的定位器.  
* 拖动目标对象的定位器：放置元素（其位置（例如，其中的最中心像素）将成为要拖动的对象的定位器）的点的定位器  

#### echo
将指定的消息打印到Selenese表中的第三个表单元格中。对于调试很有用.  
##### 参数
* message：要打印的消息  

#### edit content
设置内容可编辑元素的值，就像您在其中输入一样  
##### 参数
* locator：元素定位器.  
* value：要输入的值  

#### else
if块的一部分。如果不满足if和/或else if条件，请在此分支中执行命令。使用end命令终止分支。  

#### else if
if块的一部分。如果不满足if条件，请在此分支中执行命令。使用end命令终止分支.  
##### 参数
* 条件表达式：JavaScript表达式，它返回布尔值以用于控制流命令  

#### end
终止控制流块是否为时，为时和为时间  

#### execute script
在当前选定的框架或窗口的上下文中执行一段JavaScript。脚本片段将作为匿名函数的主体执行。要存储返回值，请使用“ return”关键字，并在值输入字段中提供变量名称  
##### 参数
* script：要运行的JavaScript代码段.  
* 变量名：不带括号的变量名  

#### execute async script
在当前选定的框架或窗口的上下文中执行JavaScript的异步代码段。脚本片段将作为匿名函数的主体执行，并且必须返回Promise。如果您使用'return'关键字，则Promise结果将保存在变量中  
##### 参数
* script：要运行的JavaScript代码段.  
* 变量名：不带括号的变量名  

#### for each
创建一个循环，为给定集合中的每个项目执行执行命令  
##### 参数
* 数组变量名称：包含JavaScript数组的变量的名称。  
* 迭代器变量名称：在循环控制流命令中迭代集合时（例如，针对每个变量）使用的变量名称  

#### if
在测试中创建条件分支。使用end命令终止分支  
##### 参数
* 条件表达式：JavaScript表达式，它返回布尔值以用于控制流命令  

#### mouse down
模拟用户按下鼠标左键（尚未释放它）。  
##### 参数
* locator：元素定位器  

#### mouse down at
模拟用户在指定位置按下鼠标左键(尚未释放它)  
##### 参数  
* locator：元素定位器.  
* 坐标字符串：指定鼠标事件相对于从定位器找到的元素的x，y位置（例如-10,20）  

#### mouse move at
模拟用户在指定元素上按下鼠标按钮（尚未释放它）.  
##### 参数  
* locator：元素定位器.  
* 坐标字符串：指定鼠标事件相对于从定位器找到的元素的x，y位置（例如-10,20）。  

#### mouse out
模拟用户将鼠标指针从指定元素移开。  
##### 参数  
* locator：元素定位器。  

#### mouse over
模拟用户将鼠标悬停在指定元素上。  
##### 参数  
* locator：元素定位器。  

#### mouse up
模拟用户释放鼠标按钮时发生的事件（例如，停止按住按钮）。  
##### 参数  
* locator：元素定位器。  

#### mouse up at
模拟当用户在指定位置释放鼠标按钮（例如，停止按住按钮）时发生的事件。  
##### 参数  
* locator：元素定位器。  
* 坐标字符串：指定鼠标事件相对于从定位器找到的元素的x，y位置（例如-10,20）。  

#### open
打开指定的URL。此URL可以是绝对路径或相对路径。  
##### 参数 
* url: 需要打开的URL（可以是相对或绝对路径）。  

#### pause
等待指定的时间。  
##### 参数 
* wait time: 需要等待的时间（以毫秒为单位）。  

#### remove selection
使用选项定位器，从多选元素的一组已选定选项中删除一个选择。  
##### 参数 
* locator: 元素定位器，识别多选框。  
* option: 一个选项定位器。通常只是一个选项标签（例如“John Smith”）。  

#### repeat if
有条件地终止“do”控制流分支。如果提供的条件表达式（conditional expression）结果为true，那么将开始do循环。否则结束循环。  
##### 参数 
* onditional expression: JavaScript表达式，返回布尔值用于控制流命令。  

#### run
从当前项目开始运行测试用例（test case）。  
##### 参数 
* test case: 项目中的测试用例名称。  

#### run script
在当前的测试窗口建立一个新的脚本（script）标签，并在命令中加入指定的文本。注意这些脚本标签引发的JS异常不由selenium管理，因此如果脚本有可能引发异常，需要将脚本放入try/catch块中。  
##### 参数 
* script: 要运行的JavaScript代码。  

#### select
使用选择定位器（select locator）从下拉菜单中选择一个元素。选项定位符提供了选择指定元素的不同方式（例如label=, value=, id=, index=）。如果没有选项定位符的前缀，则将尝试在标签上进行匹配。  
##### 参数 
* select locator: 元素定位器，用于识别下拉菜单。  
* option: 一个选项定位器。通常只是一个选项标签（例如“John Smith”）。  

#### select frame
在当前窗口中选择一个框架。可以通过从0开始的索引号（index）来选择帧数（例如使用“index=0”选择第一帧，使用“index=1”选择第二帧）。对于嵌套框架，需要多次调用此命令（对树中的每个框架都调用一次，直到达到所需框架为止）。可以使用“relative=parent”选择父框架。使用“relative=top”返回页面顶部。  
##### 参数 
* locator: 元素定位器。  

#### select window
使用窗口定位器选择弹出窗口。选择弹出窗口后，所有命令在此窗口执行。窗口定位器使用窗口句柄（handle）选择窗口。  
##### 参数 
* window handle: 代表特定页面（标签或窗口）的句柄。

#### send keys
模拟指定元素上的击键事件，类似于逐个输入值。这模拟真实用户在指定字符串中键入每个字符，同时也受到实际用户的限制，例如不能键入不可见或只读元素。适用于需要显式按键事件的动态UI小部件（例如自动完成组合框）。与简单的“类型”（type）命令不同，该命令不会替换现有内容。  
##### 参数 
* locator: 元素定位器  
*  key sequence: 要输入的按键序列，可用于发送按键（例如${KEY_ENTER}）。  

#### set speed
设置执行速度（例如，设置每个Selenium操作之后的延迟时间）。默认情况下不存在此类延迟，即延迟为0毫秒。此设置为全局设置，将影响所有测试运行，直到更改。  
##### 参数 
* wait time: 等待时间（以毫秒为单位）。  

#### set window size
设置浏览器的窗口大小。  
##### 参数 
* resolution: 使用“宽x高”的指定窗口分辨率（例如1280x800）。  

#### store
将目标字符串另存为变量，以便重复使用。  
##### 参数 
* text: 要使用的文本  
* variable name: 不带括号的变量名。  

#### store attribute
获取元素属性的值。在不同浏览器中，属性的值可能有所不同（例如“type”属性）。  
##### 参数 
* attribute locator: 元素定位符，后接@符号，然后是属性名称，例如“foo@bar”。  
* variable name: 不带括号的变量名。  

#### store json
获取json值。  
##### 参数 
* json: JavaScript对象的字符串表示形式。  
* variable name: 不带括号的变量名。  

#### store text
获取元素的文本并将其存储以备后用。适用于任何包含文本的元素。  
##### 参数 
* locator: 元素定位器。  
* variable name: 不带括号的变量名。  

#### store title
获取当前页面的标题。  
##### 参数 
* text: 要使用的文本。  
* variable name: 不带括号的变量名。  

#### store value
获取元素的值并保存备用。适用于任何输入类型元素。  
##### 参数 
* locator: 元素定位器。  
* variable name: 不带括号的变量名。  

#### store window handle
获取当前页面的句柄。  
##### 参数 
* window handle: 代表特定页面（标签或元素）的句柄。  

#### store xpath count
获取与指定xpath匹配的节点数量（例如使用“//table”会得到table数）。  
##### 参数 
* xpath:需要评估的xpath表达式。  
* variable name: 不带括号的变量名。  

#### submit
提交指定的表单（form）。这对于没有提交按钮的表单比较有用，例如单输入“搜索”表单。  
##### 参数 
* form locator: 用于定位指定表单的元素定位器。  

#### times
创建一个用于执行n次命令的循环。  
##### 参数 
* times: 控制流循环将在其块内执行命令的尝试次数。  
* loop limit: 一个可选参数，指定循环命令可以执行的最大次数。这样可以防止无限循环，默认值设置为1000。  

#### type
设置输入字段的值。同时也适用于设置组合框，复选框等。在一些情况下，值应该是指所选选项的值，而不是可见的文本。仅适用于Chrome：如果文件路径被指定，那么该路径将被上传到输入（type=file），注意不支持XPath定位器。  
##### 参数 
* locator: 元素定位器。  
* value: 输入的值。  

#### uncheck
取消一个切换按钮（单选框/复选框）。  
##### 参数 
* locator: 元素定位器。  

#### verify
断言变量是一个期望值。这个变量值会被转化为字符串用于比较。同时即使验证失败，测试也将继续。  
##### 参数 
* variable name: 不带括号的变量名.  
* expected value: 期望的变量结果（例如true,false或其他值）。  

#### verify checked
断言已选中的切换按钮（单选/复选框）。验证失败不影响测试进行。  
##### 参数 
* locator: 元素定位器。  

#### verify editable
断言指定的输入元素是否可编辑。验证失败不影响测试进行。  
##### 参数 
* locator: 元素定位器。  

#### verify element present
断言指定值不在页面上。验证失败不影响测试进行。  
##### 参数 
* locator: 元素定位器。  

#### verify not checked
断言一个切换按钮（单选/复选框）没有被选中。验证失败不影响测试进行。  
##### 参数 
* locator: 元素定位器。  

#### verify not editable
断言指定的输入元素是否不可编辑。验证失败不影响测试进行。  
##### 参数 
* locator: 元素定位器。  

#### verify not selected value
断言期望的元素没有在具有选择属性的菜单中被选中。验证失败不影响测试进行。  
##### 参数 
* select locator: 下拉菜单的元素定位器。  
* option: 选项定位符，通常只是一个选项标签（例如“ John Smith”）。  

#### verify text
断言存在一个元素的文本。验证失败不影响测试进行。  
##### 参数 
* locator: 元素定位器。  
* text: 要使用的文本。  

#### verify title
断言当前页面包含所提供文本。验证失败不影响测试进行。  
##### 参数 
* text: 要使用的文本。  

#### verify value
断言输入字段（或任何有value参数的地方）的值（空格修饰）。对于单项/复选框元素来说，根据元素是否被选中，这个值变化为“on”或“off”。验证失败不影响测试进行。  
##### 参数 
* locator: 元素定位器。  
* text: 一个完全匹配的字符串。正在支持模式匹配。详情请参见[链接](https://github.com/SeleniumHQ/selenium-ide/issues/141)


#### wait for element editable
等待元素可编辑。  
##### 参数 
* locator: 元素定位器。  
* wait time: 等待时间（以毫秒为单位）。  

#### wait for element not editable
等待元素不可编辑。  
##### 参数 
* locator: 元素定位器。  
* wait time: 等待时间（以毫秒为单位）。  

#### wait for element not present
等待目标元素不在页面上显示。  
##### 参数 
* locator: 元素定位器。  
* wait time: 等待时间（以毫秒为单位）。  

#### wait for element not visible
等待目标元素在页面上不可见。  
##### 参数 
* locator: 元素定位器。  
* wait time: 等待时间（以毫秒为单位）。  

#### wait for element present
等待目标元素在页面上显示。  
##### 参数 
* locator: 元素定位器。  
* wait time: 等待时间（以毫秒为单位）。  

#### wait for element visible
等待目标元素在页面上显示。  
##### 参数 
* locator: 元素定位器。  
* wait time: 等待时间（以毫秒为单位）。  

#### webdriver answer on visible prompt
影响当前显示的警报提示。此命令指示Selenium提供指定的回应（answer）。如果警报尚未出现，请改用“在下一个提示时回答”。  
##### 参数 
* answer: 提示弹出窗口时给出的回应。  

#### webdriver choose cancel on visible confirmation
影响当前显示的确认警报。此命令指示Selenium取消它。如果警报尚未出现，请改用“在下次确认时选择取消”。  

#### webdriver choose cancel on visible prompt
影响当前显示的警报提示。此命令指示Selenium取消它。如果警报尚未出现，请改用“在下一个提示时选择取消”。  

#### webdriver choose ok on visible confirmation
影响当前显示的确认警报。此命令指示Selenium接受它。如果尚未出现警报，请改用“在下次确认时选择确定”。  

#### while
创建一个重复执行命令的循环，只要提供的条件表达式（conditional expression）为true则进行循环。  
##### 参数 
* conditional expression: 返回用于控制流命令的结果（布尔值）的JavaScript表达式  
* loop limit: 
一个可选参数，指定循环控制流命令可以执行的最大次数。这样可以防止无限循环。默认值设置为1000。  
