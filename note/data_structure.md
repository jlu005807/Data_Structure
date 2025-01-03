# 绪论



## 数据结构的研究内容

### 数据结构主要研究**非数值计算问题 **

​           数据结构是一门研究**非数值计算**程序设计中的操作对象， 以及这些对象之间的关系和操作的学科。

> 例如:
>
> * 学生学籍管理系统
> * 人机对弈问题
> * 最短路径问题。





## 基本概念和术语



## 数据、 数据元素、 数据项和数据对象

### 数据（Date)

>数据 (Data) 是客观事物的符号表示，是所有能输入到计算机中并被计算机程序处理的**符号的总称**。
>
>* 数学计算中用到的整数和实数
>* 文本编辑中用到的字符串
>* 多媒体程序处理的图形、 图像、声音及动画等通过特殊编码定义后的数据

### 数据元素(Data Element)

>数据元素(Data Element)是数据的***基本单位***，在计算机中通常作为一个整体进行考虑和处理。 在有些情况下，数据元素也称为元素、记录等
>
>数据元素用千完整地描述一个对象
>
>* 一名学生记录
>* 树中棋盘的一个格局（状态）
>* 及图中的一个顶点

### 数据对象 (Data Object) 

> 数据对象 (Data Object) 是性质相同的数据元素的集合，是数据的一个子集。
>
> * 整数数据对象是集合N= {0, 士1' 士2,…}
> * 字母字符数据对象是集合C= {'A','B', …，'Z','a','b', …，  'z'}
> * 学生基本信息表也可以是一个数据对象

> 只要集合内元素的***性质均相同***，都可称之为一个数据对象。



## 数据结构

> 数据结构 (Data Structure) 是相互之间存在一种或多种**特定关系的数据元素的集合**。
>
> * 数据结构是带 ”结构＂ 的数据元素的**集合**
> *  “结构” 就是指数据元素之间存在的**关系**

### 逻辑结构

> 数据的逻辑结构是从**逻辑关系**上描述数据，它**与数据的存储无关**，是独立千计算机的。
>
> * 数据的逻辑结构可以看作是从具体问题抽象出来的**数学模型**。

> 数据的逻辑结构有两个要素
>
> * 数据元素
>
> * 关系  （指数据元素间的**逻辑关系**）
>
>   * 集合结构
>
>     > 数据元素之间除了 “**属于同一集合**” 的关系外，别无其他关系。例如，确定一名学生是否为 班级成员， 只需将班级看做一个集合结构。
>   * 线性结构
>     > 数据元素之间存在**一对一**的关系。例如，将学生信息数据按照其入学报到的时间先后顺序进 行排列，将组成一个线性结构。
>   * 树结构
>     > 数据元素之间存在**一对多**的关系。例如，在班级的管理体系中，班长管理多个组长，每位组长管理多名组员，从而构成树形结构。
>   * 图结构或网状结构
>     > 数据元素之间存在**多对多**的关系。例如，多位同学之间的朋友关系， 任何两位同学都可以是朋友，从而构成图状结构或网状结构。



#### 线性结构

> * 线性表（典型的线性结构，如例1.1中的学生基本信息表）
> * 栈和队列（具有特 4 l 第1章 绪论 I 殊限制的线性表，数据操作只能在表的一端或两端进行）
> * 字符串（也是特殊的线性表，其特殊性 表现在它的数据元素仅由一个字符组成）
> * 数组（是线性表的推广，它的数据元素是一个线性表）
> *  广义表（也是线性表的推广，它的数据元素是一个线性表，但不同构，即或者是单元素，或者是 线性表）

#### 非线性结构

>* 树（具有多个分支的层次结构）
>* 二叉树（具有两个分支的层次结构）
>* 有向图（一种图结构，边是顶点的有序对）
>* 无向图（另一种图结构，边是顶点的无序对）

### 存储结构

- 存储结构是逻辑结构在计算机中的存储表示
- 有两类存储结构：顺序存储结构和链式存储结构。

![image-20240716231256748](D:\Internt_of_Thing\e_book\数据结构和算法\note\assets\image-20240716231256748.png)



## 算法和算法分析

### 算法定义及其特性

- 算法 (Algorithm) 是为了解决某类问题而规定的一个**有限长的操作序列**。
-  一个算法必须满足以下五个重要特性。

1. 有穷性
2. 确定性
3. 可行性
4. 输入
5. 输出

### 评价算法优劣的基本标准

1. 正确性
2. 可读性
3. 健壮性（鲁棒性）：对有缺失、有噪声或有错误的输入数据，算法应具有较强的适应能力。
4. 高效性

### 时间复杂度

- 影响算法时间代价的最主要因素是问题规模。
- 问题规模是算法求解问题**输入量的多少**，是问题大小的本质表示，一般用整数n表示。

- 一条语句的重复执行次数称作**语句频度**(FrequencyCount)
- 而对于时间复杂度，取决于**基本运算**
- 基本运算是指算法运行过程中起**主要作用且花费时间最多**的运算

### 空间复杂度

算法在实现时所需要的辅助空间



- 接下来进入对于具体数据结构的存储和操作，只考虑算法的是实现思路





# 线性表

## 定义(逻辑结构)

- 由n(n>=0)个**数据特性相同**的元素构成的**有限序列**称为线性表
- 或者说是数据类型相同的元素组成的有限集合

- 线性表中元素的个数n(n>=0)定义为线性表的长度，n=0时称为**空表**。 
- 对千非空的线性表或线性结构，其特点是：
  1. 存在唯一的一个被称作“第一＂的数据元素；
  2. 存在唯一的一个被称作“最后一个＂的数据元素；
  3. 除第一个之外，结构中的每个数据元素均只有一个前驱；
  4. 除最后一个之外，结构中的每个数据元素均只有一个后继。

## 存储结构

### 顺序存储

- 线性表的**顺序表**示指的是用一组**地址连续的存储单元**依次存储线性表的数据元素，这种表示也称作线性表的顺序存储结构或顺序映像。
- 逻辑上相邻的数据元素，其物理次序也是相邻的
- 简单来说就是**数组**

### 链接存储

- 用**任意**一组存储单元存储线性表
- 一个存储单元除包含结点数据字段的值，还必须存放其逻辑相邻结点（前驱或 后继结点）的地址信息，即指针字段。
- **链表**

- **哨兵节点**：
  - 为便于在表头进行插入、删除操作，通常在表的前端增加一个特殊的**表头结点**，称其为哨位（哨兵）结点。

### 时空效率比较

#### 空间

- 顺序表空间来自于申请的数组空间，数组大小确定，当元素较少时，顺序表中的很多空间处于闲置状态，造成了空间的浪费；
- 链表空间是根据需要动态申请的，不存在空间浪费问题，但链表需要在每个结点上附加一个指针，从而产生额外开销

#### 时间

|        | 基于下标的查找              | 插入/删除                   |
| ------ | --------------------------- | --------------------------- |
| 顺序表 | **O(1)**按下标直接查找      | **O(n)** 需要移动若干元素   |
| 链 表  | **O(n) **从表头开始遍历链表 | **O(1) **只需修改几个指针值 |



# 栈和队列

## 栈

### 定义

- 栈(stack)是限定仅在表尾进行插入或删除操作的线性表。
- 因此，对栈来说，表尾端有其特殊含义，称为栈顶(top)
- 相应地，表头端称为栈底(bottom)。
- 不含元素的空表称为空栈。
- 栈的修改是按后进先出的原则进行的，因此，栈又称为**后进先出(LastIn First Out, LIFO)**的线性表，

### 应用

- **进制转换**：假设十进制转换为K进制：

  - 创建一个栈Stack
  - 不断除以K取余数。后生成的余数先输出，先生成的余数后输出，正好符合栈的后进先出性质。

- **括号匹配**：

  - 从左向右扫描字符串
  - 若遇到左括号：压栈 
  - 若遇到右括号：弹出栈顶的左括号与之匹配。
  - 最后判断栈空

- n对括号共有多少种可能的**合法匹配序列**：第n个卡特兰数

  - `Cn=(2n)!/(n!*n!)/(n+1)`

- **表达式求值**：（中缀表达式转变为后缀表达式）

  - 从左到右依次读入后缀表达式的每一个操作数/运算符/结束符
  - ①若读到的是操作数，将它压入栈。 
  - ②若读到的是运算符，就从操作数栈中连续弹出两个元素（操作数），进行相应的运算，并将结果压入栈中。 
  - ③读入结束符时，栈顶元素就是计算结果。

- **调度场算法**：中缀表达式转后缀表达式

  - 设置一个栈，存放运算符从左到右依次读入中缀表达式的每一个元素
  - 操作数规则：直接放入后缀表达式,注意对多位数的处理
  - 运算符规则：
    - 栈空或栈顶是左括号：压栈
    - 当前运算符优先级>栈顶运算符：压栈
    - 当前运算符优先级<=栈顶运算符：弹栈直至当前运算符 优先级>栈顶或栈空或栈顶为左括号（期间弹出的运算符顺序依次放入后缀表达式），再把当前运算符压栈
  - 括号规则： (1) 遇到左括号：压栈 (2) 遇到右括号：弹栈直至左括号 
  - 结束符规则：弹栈至栈空

- **栈混洗**：给定入栈序列，模拟出栈序列

  - n个元素的栈混洗总数，即n对括号的匹配序列，卡特兰数*(n+1)

  - n个元素的栈混洗合法出栈序列，即n对括号的合法匹配序列，卡特兰数*(n+1)

## 队列

### 定义

- 队列(queue)是一种**先进先出(First In First Out, FIFO)**的线性表
- 允许插入的一端称为队尾(rear), 允许删除的一端则称为队头(front)。

### 应用

- BFS广度优先搜索

- 栈和队列都需要注意的一点是top和rear指针是指向元素还是下一个空位置



# 数组和矩阵

## 数组

### 多维数组的存储和寻址：

- 已知数组`A[a][b][c][d]`,每个元素占C个存储单元
-  数组元素`A[i] j][k][l]`的存储地址：
  - 行优先:`Loc(A)+( i*b*c*d + j*b*d + k*d + l )*C`
  - 列优先:`Loc(A)+( i + j*a + k*a*b + l*a*b*c )*C`

### 矩阵的压缩存储

- 压缩存储需考虑2个问题
- 需要多大存储空间：数组d[ ]需要多少元素 
- 地址映射：矩阵的任意元素M(i, j)在一维数组d[ ]中的位置（下标）， 即把矩阵元素的下标映射到数组d的下标

1. **对角矩阵的压缩存储**
   1. 对于一个n*n的对角矩阵，至多只有n个非0元素，因此只需存储n个对角元素
   2. `M( i , i ) -> d[ i ]`

2. **(下）三角矩阵的压缩存储**
   1. 以按行优先方式压缩存放在一维数组d，d需要`n(n+1)/2`个元素
   2. `M(i, j)= d[k]=d[i(i−1)/2 + (j−1)]`

3. 对称矩阵M的压缩存储
   1. 对称矩阵中M(i, j)与M(j, i)的信息相同，只需存储M的下三角部分的元素信息。
   2. 对于对称矩阵中的下三角元素`M(i, j) (i>=j)` :
      1. `i < j，M(i, j)=d[k]，k = i(i−1)/2 + (j−1)`
   3. 对于上三角元素`M(i, j) (i<j)`:元素值与下三角矩阵中的 元素M(j,i)相同
      1. `i < j, M(i, j)=M(j, i)=d[q]， q= j(j−1)/2 + (i−1)`

4. **三对角矩阵M的压缩存储**
   1. 方阵Mn*n中任意元素M(i, j)，当| i - j | >1时，有M(i, j) =0， 则 M称为三对角矩阵。
   2. 需要3*n-2个存储单位
   3. 对于非零元素：即`| i-j | <=1, M(i,j) = d[2*i + j - 3]`

5. 稀疏矩阵的压缩存储

   1. 非零元素的个数远小于零元素的个数
   2. 三元组结点来存储矩阵的每个非零元素aij，其中i和j为元素的行号和列号，即`node(i,j,aij)`
   3. 十字链表:数据,该结点所在行 ,该结点所在列 ,指向左侧相邻非零元素的指针 ,指向上方相邻非零元素的指针,即`node(row,col,value,left,up)`
   4. 双向十字链表

   

# 字符串

## 定义

- 串(string)(或字符串）是由零个或多个字符组成的**有限序列**
- 串中字符的数目n称为串的长度
- 零个字符的串称为空串(null string) , 其长度为零

## 应用

- 模式匹配
  - KMP
  - 注意next数组的意义以及和失败函数fail的区别



# 树

- 一棵树是结点的一个有限集合T。
- 若T空，则称为空树。 
- 若T非空，则：
  - 有一个被称为根的结点，记 为root(T) ； 
  - 其余结点被分成m(m >=0) 个 不相交的非空集合T1,T,…,Tm， 且T1, T2, …, Tm也都是树，其 称为root(T)的**子树**。(递归结构)

- 相关术语
  - 度 ：一个结点的度指该结点的子结点的数目。一棵树的度为各结点的度的最大值。
  - 叶结点：度为0的结点，即没有孩子的结点。
  - 分支结点 ：度大于0的结点，即非叶结点
  - 边：树中结点间的连线
  - 层数/深度：根结点层数为0，其余结点的层数为其父结点的层数加1。
  - 树的高度/深度：树中结点的最大层数
  - 结点的高度：以该结点为根的子树的高度

- 对于二叉树
- 二叉树中第i层至多有2^i个结点，i>=0
- 高度为k的二叉树中至多有`2^(k+1)-1 (k>=0)`个结点
- 在n个结点构成的二叉树中，若叶结点个数为n0 ，度为2的结点个数为n2 ，则有：`n0 =n2 ＋1`
- 特殊二叉树
  - 满二叉树
  - 完全二叉树

- 树的遍历
  - 前序遍历
  - 中序遍历
  - 后序遍历

- 树和二叉树的转换（兄弟儿子表示法）

## 应用

- 先根序列个数为n的不同二叉树的个数为卡特兰数
- 线索二叉树
- 哈夫曼树
  - 依次找到最小的两个节点组成一棵树直到所有节点都有根节点
- 并查集
  - 压缩路径
  - 大树并入小树



# 图

## 存储结构

- 边存储
- 邻接表（稀疏图）
- 邻接矩阵（稠密图）





## 应用

- DFS:深度优先搜索

  - 非递归利用栈

- BFS:广度优先搜索

  - 非递归利用队列（类似树的层次遍历）
  - 可用于单源无权（权值为1）最短路

- 拓扑序列：AOV网是一个有向无环图，也就是说可以用于证明图是否有环

  1. 选择一个入度为0的顶点并输出

  2. 删除该顶点及该顶点引出的所有边

  3. 执行①②，直至所有顶点已输出，或图中剩余顶点 入度均不为0（说明存在环，无法继续拓扑排序）
  4. 对于任何无环的AOV网，其顶点均可排成拓扑序列， 其拓扑序列**未必唯一**
  5. 拓展：DFS可以输出拓扑序的逆序

- 关键路径：完成整个工程所需的最短时间取决于从源点到汇点的最长路径长度

  - 关键活动：活动 的最早开始时间等于活动 A 的最迟开始时间， 即`l(i)＝e(i)`
  - 关键路径：由关键活动组成的路径，亦即源点到汇点的最长 路径，可能不止一条

  1. 对AOE网求各顶点vj的最早发生时间ve(j)
  2. 求各顶点vj的最迟发生时间vl(j)；
  3. 求出各活动ai的最早开始时间e(i)和 最迟开始时间l(i)，若e(i)=l(i)，则ai是关键活动
  4. 具体算法
     1. 拓扑排序，若网中有环则终止算法，按拓扑 序求出各顶点的最早发生时间ve
     2. 按逆拓扑序求各顶点的最迟发生时间vl
     3. 根据ve和vl的值，求各活动的最早开始时间e与最迟开始时 间l，若e=l，则对应活动是关键活动

- 最短路径
  - 无权图的单源最短路径问题：BFS
    - BFS过程中，当访问某个顶点时，就确定了该点与源点的最 短距离
    - 通过BFS，从源点开始由近及远求各顶点的最短路径v
  - 正权图的单源最短路径问题：Dijkstra算法
    - 找到各个局部最优路（任意最短路的前缀，也是一条最短路）
    - 初始化起点到其他点距离
    - 找局部最优路
    - 从局部最优路更新到其他点的距离
    - 重复直到所有点的最优路找到
    - 可以利用优先队列（斐波那契堆）优化找局部最优路的步骤
  - 正权图的多源最短路径问题
    - 多次Dijkstra算法
    - Floyd算法（多用于邻接矩阵）
      - 在一段路径里尝试插入一个点找到更短路

- 最小支撑树：边权之和最小的支撑树称为G的最小支撑树

  -  Prim算法（加点法）
    - 选择任一点u做为起点，放入集合S，即令S={u}(u属于V)；
    - 找最小跨集合边(u, v) ，即端点分别属于集合S和V-S且权值 最小的边，将该边加入最小支撑树，并将点v放入S；
    - 执行②，直至S=V
  - Kruskal算法（逐边加入）
    - 在G中选择权值最小的边，并将此边从G中删除
    - 若该边加入T后不产生环（即此边的两个端点在T的不同连 通分量中），则将此边加入T中，从而使T减少一个连通分 量，否则本步骤无操作，对于是否产生环可以利用并查集
    - 重复①②直至T中仅剩一个连通分量

  

# 排序

- 内排序
  - 插入排序
    - 直接插入
    - 选择排序
  - 交换排序
    - 冒泡
    - 快速
  - 堆排序
  - 分布排序
    - 基数排序
    - 计数排序
    - 桶排序
  - 堆排序



# 查找

- 顺序查找
- 对半查找
- 斐波那契查找
- 插值查找
- 分块查找

