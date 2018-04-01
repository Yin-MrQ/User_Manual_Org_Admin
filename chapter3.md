## 个人工作区

用户在Notebook进行数据分析的过程中，如果生成了新的文件，这些文件将会保存在**个人工作区**里面。这个工作区相当于一个磁盘，用户可在Notebook中的Code Cell中输入Linux命令方式进行访问。

### 工作区目录
工作区分为input和work两个目录，**其中work目录下的内容可以持久化存储**。

* input目录：
  * 作用：挂载当前项目所使用的数据集文件
  * 访问：```ls /home/kesci/input/```
  
* work目录：
  * 作用：持久化存储数据分析中产生的文件
  * 访问：```ls /home/kesci/work/```

温馨提示：用户可以通过Linux指令将需要持久化存储的文件移至该目录下。

### 工作区常用命令

* ls
    * 作用：查看特定路径下的文件/文件夹
    * 示例：```ls /home/kesci/input/```
* rm
    * 作用：删除特定路径下的文件/文件夹
    * 示例：```rm /home/kesci/work/tmp.txt``` 
* mkdir 
    * 作用：创建特定路径下的文件夹
    * 示例： ```mkdir /home/kesci/myfolder/```
* mv:
    * 作用：移动原路径下的文件/文件夹到新路径下
    * 示例：```mv /home/kesci/work/tmp.txt /home/kesci/myfolder/```
* cp:
    * 作用：拷贝原路径下的文件/文件夹到新路径下
    * 示例：``` cp /home/kesci/work/tmp.txt /home/kesci/myfolder/```
