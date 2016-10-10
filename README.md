# **Lab2主题：版本控制&文档**
## **Description**
分布式操作层（DOL）是一个编译并行应用程序的软件开发框架，它可以指定基于Kahn过程网络计算模型和以SystemC的模拟引擎为特色的应用。此外，DOL还提供了基于XML的规范格式来描述多处理器系统上包括绑定和映射的并行应用程序的实现。
## **How to install**
### 步骤
####1.使用虚拟机安装Ubuntu
####2.安装环境
  a)sudo apt-get update
  b)sudo apt-get install ant
  c)sudo apt-get install openjdk-7-jdk
  d)sudo apt-get install unzip
####3.下载文件
  a)sudo wget http://www.accellera.org/images/downloads/standards/systemc/systemc-2.3.1.tgz
  b)sudo wget http://www.tik.ee.ethz.ch/~shapes/downloads/dol_ethz.zip
####4.解压文件
  a)mkdir dol（新建dol文件夹）
  b)unzip dol_ethz.zip -d dol（将dolethz.zip解压到 dol文件夹中）
  c)tar -zxvf systemc-2.3.1.tgz（解压systemc）
####5.编译systemc
  a)cd systemc-2.3.1（进入systemc-2.3.1的目录）
  b)mkdir objdir（新建临时文件夹objdir）
  c)cd objdir
  d)../configure CXX=g++ --disable-async-updates（运行configure）
  e)sudo make install（编译）
  f)cd ../dol
    修改build_zip.xml文件
####6.编译dol
  a)ant -f build_zip.xml all

## **Experimental experience**
  总的来说，DOL环境配置没有什么大的问题，就是在安装过程中直接在ubuntu中在网站下载的压缩包可能出现文件损坏的情况（网络来源以及网络不稳定），所以在第一次完成试验时总是提示文件缺失，最后直接在外部下载完毕后拖进虚拟机完成后续步骤。