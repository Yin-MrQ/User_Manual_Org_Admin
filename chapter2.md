# Kernel(计算环境)
Kernel是Notebook对应的计算环境。Kernel中预先加载了**Python2 & 3** 和 **R** 等主流编程语言对应的**常用数据分析框架**和**工具包**，用户可直接导入数据，通过Notebook编写代码，和Kernel开始数据分析。

![image description](image/kernel.png)
## Kernel类型
* Python3 Kernel   
K-Lab 提供 Python 3.5版本的 Python Kernel，并支持大部分的主流数据分析工具包。    
```Python
import sys
print (sys.version) # 3.5.2
```
* Python2 Kernel   
K-Lab 提供 Python2.7版本的 Python Kernel，并支持基础的数据分析工具包。    
```python
import sys
print sys.version # 2.7.9
```
* R Kernel 
K-Lab 提供R 3.3.2 版本的 R kernel，并支持大部分的 R 语言主流数据分析工具包。
```R
R.version.string # 3.3.2
```

友情提示：科赛建议 Python 用户在 K-Lab 上使用 Python3 进行编程分析。

## Kernel内置工具包
K-Lab Kernel支持用户在与Kernel相连的Notebook中输入指令查看、安装和更新工具包。 
### 查看工具包
用户可在Notebook的Code Cell中键入相应指令查看预置的工具包。
* Python2 Kernel    
```
%%bash
pip2 list --format=columns  #查看Kernel下所有预置的工具包
pip2 show package_name      #查看Kernel是否有某个工具包
```
* Python3 Kernel
```
%%bash
pip list --format=columns  #查看Kernel下所有预置的工具包
pip show package_name      #查看Kernel是否有某个工具包
```
* R Kernel

### 安装工具包
用户可在Notebook的Code Cell中键入相应指令安装所需要的工具包，也可以通过[帮助中心](https://www.kesci.com/apps/home/workspace/help)下的意见反馈`向科赛网提出工具包安装需求，我们将在2个工作日内给出答复。
* Python2 Kernel
```
%%bash
pip2 install package_name==version #如果不注明version则自动安装最新版本
```
* Python3 Kernel
```
%%bash
pip install package_name==version #如果不注明version则自动安装最新版本
```
* R Kernel
```
install.packages(package_name)
```

友情提示：手动安装好工具包后，请刷新页面，Notebook所对应的Kernel将完成工具包部署。

### 升级工具包
用户可在Notebook的Code Cell中键入相应指令升级所需要的工具包，也可以通过[帮助中心/K-Lab工具包页面](https://www.kesci.com/apps/home/workspace/help)下的`包安装反馈`向科赛网提出工具包升级需求，我们将在2个工作日内给出答复。
* Python2 Kernel
```
%%bash
pip2 install package_name --upgrade
```
* Python3 Kernel
```
%%bash
pip install package_name --upgrade
```
友情提示：手动升级好工具包后，请刷新页面，Notebook所对应的Kernel将完成工具包部署。

## Kernel计算资源
K-Lab为每位用户分配**2核8G**的独享计算资源，为了让计算资源有效分配，用户单次使用时长限制为**2小时**，超过2小时 Kernel 将自动断开，用户可以通过刷新手动连接 Kernel 分配到新的计算资源，继续开展分析工作，剩余可用时间在右上角显示。

![image description](image/kernel-time.png)