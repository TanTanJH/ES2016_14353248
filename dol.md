# **Lab3主题：DOL实例分析&编程**

## **DOT截图**
![task1.png](https://github.com/ES201614353248/ES2016_14353248/blob/master/task1.png)
![task2.png](https://github.com/ES201614353248/ES2016_14353248/blob/master/task2.png)

## **修改步骤**
###Task1：
> * 1.打开example2.xml文件
> * 2.将<variable value="3" name="N"/>改为<variable value="2" name="N"/>
> * 3.进入Terminal；cd dol/build/bin/main；ant -f runexample.xml -Dnumber=2
> * 4.检查consumer的值
###Task2：
> * 1.打开example1的src文件中的square.c文件
> * 2.将square_fire中的i=i*i改为i=i*i*i
> * 3.进入Terminal；cd dol/build/bin/main；ant -f runexample.xml -Dnumber=1
> * 4.检查consumer的值

## **实验感想**
####实验过程要注意的是Lab1已经跑过一次example1，并因此在build的相应文件目录下有了测试结果。然而重新测试不会覆盖已有的测试结果，所以虽然代码改变了，结果依旧没有发生变化，只要把旧文件删除再重新运行就可以得到新测试结果；
####个人认为这次实验最大的收获是理解了DOL不同文件的意义，知道各种.c、.h和.xml文件分别代表什么，以及这些文件之间的联系，对DOL实例编程有了初步的了解