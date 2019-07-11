# Searching-practise
廖明宏的数据结构与算法中查找一章的练习。
其中有代码风格不统一，复用率低，不规范等问题，这是因为1.我想多试试几种不同的方法；2.因为是小项目，想省点时间去复习，所以有时候就粘贴了，提高复用率以后会多研究；3.规范慢慢改进吧。这里只是给自己一个记录和问题总结，当然欢迎交流。

searchingH.h
  定义结构体，数据集、结点等。

SearchClass.h
  定义了一个SearchClass类，作为重点的搜索算法在这里。

LinearSearch.cpp
  只定义了一个简单的线性表搜索函数，只是为了试一下vs2019的创建类的功能。

SearchingPractice.cpp
  测试的地方，写得随便了点不好意思，因为自己也在研究，所以会这个地方改下，那个地方改下。基本就是临时创建一个表或树，再测试相关查找、插入、删除函数。
  
 7-11 update
 加入平衡二叉树（avlTree）的相应算法。
 平衡二叉树大部分算法和二叉查找树大体一样，就是添加上了旋转调整部分。
 不过在编写删除算法的时候还是遇到了一些困难，测试时发现出现了不平衡结点但结果并未调整的情况。
 于是在遍历算法中加入输出结点高度的语句，运行发现叶结点高度都是0，本来设计应该是空指针情况是0，叶结点高度为1。问题的关键在于结点默认的初始化高度为0，默认初始化高度值改为1即可。
 *另外重载了records结构体的初始化函数，各位要测试的时候注意不要忽略了。*
AVLTree类的中主要是插入和删除算法，搜索算法和BST一样懒得重写一遍了。
这部分的内容有点长，可能要考虑下之后再建比较大的类的时候要专门创建一个类的头文件。

边学边做，还在进行中
