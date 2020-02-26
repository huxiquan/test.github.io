#### open
打开指定的URL。此URL可以是绝对路径或相对路径。  
```参数：```url: 需要打开的URL（可以是相对或绝对路径）。  

#### pause
等待指定的时间。  
```参数：```wait time: 需要等待的时间（以毫秒为单位）。  

#### remove selection
使用选项定位器，从多选元素的一组已选定选项中删除一个选择。
```参数：```locator: 元素定位器，识别多选框。 option: 一个选项定位器。通常只是一个选项标签（例如“John Smith”）。  

#### repeat if
有条件地终止“do”控制流分支。如果提供的条件表达式（conditional expression）结果为true，那么将开始do循环。否则结束循环。  
```参数：```onditional expression: JavaScript表达式，返回布尔值用于控制流命令。  

#### run
从当前项目开始运行测试用例（test case）。  
```参数：```test case: 项目中的测试用例名称。  

#### run script
在当前的测试窗口建立一个新的脚本（script）标签，并在命令中加入指定的文本。注意这些脚本标签引发的JS异常不由selenium管理，因此如果脚本有可能引发异常，需要将脚本放入try/catch块中。  
```参数：```script: 要运行的JavaScript代码。  

#### select
使用选择定位器（select locator）从下拉菜单中选择一个元素。选项定位符提供了选择指定元素的不同方式（例如label=, value=, id=, index=）。如果没有选项定位符的前缀，则将尝试在标签上进行匹配。  
```参数：```select locator: 元素定位器，用于识别下拉菜单。 option: 一个选项定位器。通常只是一个选项标签（例如“John Smith”）。  

#### select frame
在当前窗口中选择一个框架。可以通过从0开始的索引号（index）来选择帧数（例如使用“index=0”选择第一帧，使用“index=1”选择第二帧）。对于嵌套框架，需要多次调用此命令（对树中的每个框架都调用一次，直到达到所需框架为止）。可以使用“relative=parent”选择父框架。使用“relative=top”返回页面顶部。  
```参数：```locator: 元素定位器。  

#### select window
使用窗口定位器选择弹出窗口。选择弹出窗口后，所有命令在此窗口执行。窗口定位器使用窗口句柄（handle）选择窗口。  
```参数：```window handle: 代表特定页面（标签或窗口）的句柄。

#### send keys
模拟指定元素上的击键事件，类似于逐个键入值。这模拟真实用户在指定字符串中键入每个字符，同时也受到实际用户的限制，例如不能键入不可见或只读元素。适用于需要显式按键事件的动态UI小部件（例如自动完成组合框）。与简单的“类型”（type）命令不同，该命令不会替换现有内容。  
```参数：```locator: 元素定位器。 key sequence: 要输入的按键序列，可用于发送按键（例如${KEY_ENTER}）。  

#### set speed
设置执行速度（例如，设置每个Selenium操作之后的延迟时间）。默认情况下不存在此类延迟，即延迟为0毫秒。此设置为全局设置，将影响所有测试运行，直到更改。  
```参数：```wait time: 等待时间（以毫秒为单位）。  

#### set window size
设置浏览器的窗口大小。  
```参数：```resolution: 使用“宽x高”的指定窗口分辨率（例如1280x800）。  

#### store
将目标字符串另存为变量，以便重复使用。  
```参数：```text: 要使用的文本。 variable name: 不带括号的变量名。  

#### store attribute
获取元素属性的值。在不同浏览器中，属性的值可能有所不同（例如“type”属性）。  
```参数：```attribute locator: 元素定位符，后接@符号，然后是属性名称，例如“foo@bar”。 variable name: 不带括号的变量名。  

#### store json
获取json值。  
```参数：```json: JavaScript对象的字符串表示形式。 variable name: 不带括号的变量名。  

#### store text
获取元素的文本并将其存储以备后用。适用于任何包含文本的元素。  
```参数：```locator: 元素定位器。 variable name: 不带括号的变量名。  

#### store title
获取当前页面的标题。  
```参数：```text: 要使用的文本。 variable name: 不带括号的变量名。  

#### store value
获取元素的值并保存备用。适用于任何输入类型元素。  
```参数：```locator: 元素定位器。 variable name: 不带括号的变量名。  

#### store window handle
获取当前页面的句柄。  
```参数：```window handle: 代表特定页面（标签或元素）的句柄。  

#### store xpath count
获取与指定xpath匹配的节点数量（例如使用“//table”会得到table数）。  
```参数：```xpath:需要评估的xpath表达式。 variable name: 不带括号的变量名。  

#### submit
提交指定的表单（form）。这对于没有提交按钮的表单比较有用，例如单输入“搜索”表单。  
```参数：```form locator: 用于定位指定表单的元素定位器。  

#### times
创建一个用于执行n次命令的循环。  
```参数：```times: 控制流循环将在其块内执行命令的尝试次数。 loop limit: 一个可选参数，指定循环命令可以执行的最大次数。这样可以防止无限循环，默认值设置为1000。  

#### type
设置输入字段的值。同时也适用于设置组合框，复选框等。在一些情况下，值应该是指所选选项的值，而不是可见的文本。仅适用于Chrome：如果文件路径被指定，那么该路径将被上传到输入（type=file），注意不支持XPath定位器。  
```参数：```locator: 元素定位器。 value: 输入的值。  

#### uncheck
取消一个切换按钮（单选框/复选框）。  
```参数：```locator: 元素定位器。  

#### verify
断言变量是一个期望值。这个变量值会被转化为字符串用于比较。同时即使验证失败，测试也将继续。  
```参数：```variable name: 不带括号的变量名。 expected value: 期望的变量结果（例如true,false或其他值）。  

#### verify checked
断言已选中的切换按钮（单选/复选框）。验证失败不影响测试进行。  
```参数：```locator: 元素定位器。  

#### verify editable
断言指定的输入元素是否可编辑。验证失败不影响测试进行。  
```参数：```locator: 元素定位器。  

#### verify element present
断言指定值不在页面上。验证失败不影响测试进行。  
```参数：```locator: 元素定位器。  

#### verify not checked
断言一个切换按钮（单选/复选框）没有被选中。验证失败不影响测试进行。  
```参数：```locator: 元素定位器。  

#### verify not editable
断言指定的输入元素是否不可编辑。验证失败不影响测试进行。  
```参数：```locator: 元素定位器。  

#### verify not selected value
断言期望的元素没有在具有选择属性的菜单中被选中。验证失败不影响测试进行。  
```参数：```select locator: 下拉菜单的元素定位器。 option: 选项定位符，通常只是一个选项标签（例如“ John Smith”）。  

#### verify text
断言存在一个元素的文本。验证失败不影响测试进行。  
```参数：```locator: 元素定位器。 text: 要使用的文本。  

#### verify title
断言当前页面包含所提供文本。验证失败不影响测试进行。  
```参数：```text: 要使用的文本。  

#### verify value
断言输入字段（或任何有value参数的地方）的值（空格修饰）。对于单项/复选框元素来说，根据元素是否被选中，这个值变化为“on”或“off”。验证失败不影响测试进行。  
```参数：```locator: 元素定位器。 text: 一个完全匹配的字符串。正在支持模式匹配。详情参见<https://github.com/SeleniumHQ/selenium-ide/issues/141>  

#### wait for element editable
等待元素可编辑。  
```参数：```locator: 元素定位器。 wait time: 等待时间（以毫秒为单位）。  

#### wait for element not editable
等待元素不可编辑。  
```参数：```locator: 元素定位器。 wait time: 等待时间（以毫秒为单位）。  

#### wait for element not present
等待目标元素不在页面上显示。  
```参数：```locator: 元素定位器。 wait time: 等待时间（以毫秒为单位）。  

#### wait for element not visible
等待目标元素在页面上不可见。  
```参数：```locator: 元素定位器。 wait time: 等待时间（以毫秒为单位）。  

#### wait for element present
等待目标元素在页面上显示。  
```参数：```locator: 元素定位器。 wait time: 等待时间（以毫秒为单位）。  

#### wait for element visible
等待目标元素在页面上显示。  
```参数：```locator: 元素定位器。 wait time: 等待时间（以毫秒为单位）。  

#### webdriver answer on visible prompt
影响当前显示的警报提示。此命令指示Selenium提供指定的回应（answer）。如果警报尚未出现，请改用“在下一个提示时回答”。  
```参数：```answer: 提示弹出窗口时给出的回应。  

#### webdriver choose cancel on visible confirmation
影响当前显示的确认警报。此命令指示Selenium取消它。如果警报尚未出现，请改用“在下次确认时选择取消”。  

#### webdriver choose cancel on visible prompt
影响当前显示的警报提示。此命令指示Selenium取消它。如果警报尚未出现，请改用“在下一个提示时选择取消”。  

#### webdriver choose ok on visible confirmation
影响当前显示的确认警报。此命令指示Selenium接受它。如果尚未出现警报，请改用“在下次确认时选择确定”。  

#### while
创建一个重复执行命令的循环，只要提供的条件表达式（conditional expression）为true则进行循环。  
```参数：```conditional expression: 返回用于控制流命令的结果（布尔值）的JavaScript表达式。 loop limit: 
一个可选参数，指定循环控制流命令可以执行的最大次数。这样可以防止无限循环。默认值设置为1000。  
