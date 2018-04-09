# 磁盘空间
K-Lab为每个用户提供一个独享的磁盘空间，用户可以在 `/home/kesci/`目录下进行文件读写。其中`/home/kesci/work/`为个人工作区目录，`/home/kesci/input/`为数据集挂载目录。
![worksaoce](image/workspace.png)

## 个人工作区
K-Lab为每个用户提供 500 Mib 的云端持久化存储空间作为个人工作区，访问路径为 `/home/kesci/work/`，写到该目录下的文件将被持久化存储，方便用户保存阶段性成果。

个人工作区可跨项目共享，即打开不同的K-lab项目时将访问同一work目录，方便不同项目的中间文件调用。用户在关闭K-Lab时触发工作区文件的自动存储，重新打开K-Lab时恢复上次保存的工作区文件。

* 友情提醒：`/home/kesci/work/`目录下不得存放超过500 Mib的文件，超过500 Mib将导致工作区持久化失败，工作区用量可以在监控区查看。

## 数据集挂载目录
用户挂载的数据集将会放在 `/home/kesci/input/`目录下，挂载的数据集信息可以在侧边栏快速查看，更多数据集功能详见[数据集](chapter4.md)


## 常用文件操作命令

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
