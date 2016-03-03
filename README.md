# 算法和数据结构
本文件夹里存储了主要的算法和常见的数据结构。所有算法以及数据结构都是用C++实现的。

==============
###AVL Tree(AVL平衡二叉树)
在二叉查找树的基础上，通过四种操作RR，LL，LR和RL，使得左右子书深度之差不超过2。这样，在查找的时候，算法时间复杂度能维持在一个O(logN)的稳定的时间。

==============
###B_Tree(B树)
B树是常见的储存数据结构。每个非叶子节点可以有n个关键字，同时有n+1棵子树。包括插入，查找，删除三种操作。

==============
###calculate(计算器)
输入一个数学表达式，采用中缀表示的形式输入。程序输出表达式对应的逆波兰表达式，并同时利用逆波兰表达式计算表达式的结果。

==============
###Dijkstra(Dijkstra算法)
Dijkstra算法是一个动态规划算法，计算带权有向图中单源最短路径距离。图由邻接矩阵表示，每次更新利用最小堆结构返回最近的节点。

==============
###Disjoint Set(并查集)
利用树结构存储数据，如果两个节点具有某种关系，则合并两个所在的树。最后属于同一棵树的节点处在一个集合里。

==============
###Floyd(Floyd算法)
Floyd算法也是带权有向图上的动态规划算法，计算图中任意两点之间的最短路径距离。算法采用三层循环，所以时间复杂度为n的三次方。算法先固定一个点k作为中间节点，如果点i到点k距离加上点k到点j的距离小于之前计算的点ij之间的距离，则更新点ij之间的距离。

==============
###Forest(森林和二叉树相互转换)
森林和二叉树之间的转换很简单，在二叉树中，每个节点的左儿子是森林中该节点的最左儿子，而节点的右儿子是森林中该节点的兄弟节点。

==============
###Graph(图的遍历算法)
最基本的图遍历算法就是深度优先和广度优先算法。深度优先，访问节点的某个相邻点（该节点未被访问过）并将节点入栈，如果一个节点没有相邻节点或者所有相邻节点都被访问则弹栈，访问栈顶节点的下一个相邻点；广度优先，访问节点，并将节点的所有未访问过相邻点入队列，弹出队列第一个元素，访问该节点并将该节点的所有未访问过相邻点入队列。

==============
###Hash(散列表)
本文件主要实现了三种常见的散列表：闭散列表，开散列表和外散列表。同时，比较了三种散列表的查找时间。闭散列表，当插入冲突时，则按照某种规则选择下一个存储位置；开散列表，当插入冲突时，则采用链表结构，插入到该位置上的链表的末尾；外散列表，和开散列表差不多，差别是外散列表中散列表不存储数据，存储链表头指针。

==============
###Heapify(堆排序)
本程序实现用堆排序算法排序int型数据。算法的核心在于维护一个最小堆结构。

==============
###Huffman(哈弗曼树)
构建huffman树，并通过huffman树来获得字符的huffman编码。

==============
###Josephus(约瑟夫环问题)
主要用队列这种数据结构就可解决此问题，本程序实现了队列的主要操作。

==============
###Kruskal(Kruskal算法)
这是一个求加权联通图的最小生成树的算法。这是一个贪心算法，每次选择权重最小的边，如果该边和之前已选中的边不构成环，则将该边加入生成树中。

==============
###memory allocation(内存分配)
通过链表结构将零碎的内存空间链接在一起，程序用数值模拟物理内存，同时模拟的内存分配和内存释放操作。

==============
###Prim(Prim算法)
图算法中的一种，用于求解加权联通图的最小生成树。同样这也是一个贪心算法，初始化G为图中任意一点，从图中选出和G相连的权值最小的边（边的一个端点属于G，另一个端点不属于G），将该边加入G中，直到G包含原图的所有节点。

==============
###Sort(排序算法)
该文件包含常见的排序算法，并在同一个数据集上比较了不同排序算法所消耗的时间。实现的排序算法以及排序时间：

|排序算法 |时间|
|:---|:---|
|冒泡排序 |8469ms|
|插入排序 |3281ms|
|希尔排序 |16ms|
|选择排序 |3656ms|
|快排     |<1ms|
|归并排序 |16ms|
|堆排序   |15ms|
|基数排序 |32ms|

