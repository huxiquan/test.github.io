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
模拟指定元素上的击键事件。