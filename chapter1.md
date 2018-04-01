# Notebook(编程环境)
Notebook是用户登录科赛网并打开K-Lab后，在浏览器端所看到的交互式编写界面，由**Header**、**Code Cell**、**Markdown Cell**和**代码收藏区**组成。
## Header
Notebook页面上端构成了Header，包含了项目名称、菜单栏和工具栏。用户在编辑cell时,即使Notebook页面下滑，Header也会保持在页面的最顶端。项目名称可以被用户修改。工具栏和菜单栏包含了各类不同的操作命令和工具方便用户对Notebook进行编辑。
![image description](image/header.png) 

## Code Cell
Code Cell是Notebook的代码编写单元。用户在Code Cell内编写代码(目前科赛网支持**Python2 & 3**和**R**等主流编程语言)，代码由后端的Kernel运行，并返回结果到Code Cell。通过这样一个工作流，用户来**解决数据分析中如数据导入、模型搭建、数据可视化、参数调优等问题**。    

![image description](image/code-cell.png)
Code Cell有**编辑模式**和**命令模式**两种状态，状态可以相互切换：编辑模式下，按`Enter`键进入命令模式；命令模式下，按`Esc`键进入编辑模式。

* 编辑模式：表示该cell允许被编辑，界面上显示cell单元框线为绿色，即用户可以在cell中键入代码或注释。
 ![image description](image/code-cell-green.png)

* 命令模式：表示该cell允许被执行，界面上显示cell的单元框线为蓝色，即用户可以通过点击`运行`按钮或快捷键`Shift + Enter`来运行cell。
  ![image description](image/code-cell.png)




## Markdown Cell
Markdown Cell是K-Lab的文本编辑单元，用户通过在Markdown Cell中输入Markdown格式的文本，来**完成数据分析中的报告撰写任务**。

Markdown Cell也有**编辑模式**和**命令模式**两种状态，编辑模式下，按`Enter`键进入命令模式；命令模式下，按`Esc`键进入编辑模式。
* 编辑模式：表示该cell允许被编辑，界面上显示cell单元框线为绿色，即用户可以在cell中键入Markdown格式文本。

  ![image description](image/markdown-cell-green.png)
* 命令模式：表示该cell允许被执行，界面上显示cell的单元框线为蓝色，即用户可以通过点击`运行`按钮或快捷键`Shift + Enter`来完成Markdown文本渲染。
 ![image description](image/markdown-cell-blue.png)  

更多K-Lab Makrdown使用示例，[请参考链接](https://www.kesci.com/static/markdown_guide.html)。

**温馨提示**：    

<div class="alert alert-success">
按下Enter键或在cell的编辑区内单击鼠标，进入编辑模式。
</div>
<div class="alert alert-success">
按下Esc键或在cell的编辑区外单击鼠标，进入命令模式。
</div>
<div class="alert alert-warning">
请勿尝试在code cell运行时对该cell进行编辑。
</div>

## 代码收藏区
在Notebook页面左侧点击星标按钮，即能看见代码收藏区。分为**公有库**和**我的收藏**。
* 公有库：收集的常用的代码可供用户使用。        
![image description](image/code-storage.png)


* 我的收藏：用户私人收藏的代码。
![image description](image/code_my_favorite.png)