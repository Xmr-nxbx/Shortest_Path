# 关于此文件的编写  
此文件`最短路径问题`主界面是我编写，是为了完成老师要求布置作业（被迫）  
要求的算法有以下：  

* 深度优先搜索 
* 广度优先搜索
* 带启发式的搜索（A*）

***此程序未完成,还需要努力***  

# 关于算法
对于前两个基本搜索就不做多解释  

#### 启发式搜索  
利用引导信息解决问题  
>用于评价节点重要性的函数称为估价函数，其一般形式为  
```f(x) = g(x) + h(x)```  
式中：g(x)为从初始节点到节点x付出的实际代价；h(x)为从节点x到目标节点的最优路径的估计代价。  
启发性信息主要体现在h(x)中，其形式要根据问题的特性来确定。  

对于路径问题,就可以联想到节点代价可以算作起始位置到本位置的代价`g(x)`。  

我们知道，两个点的直线距离最短，便可以以此条件，假设到目标距离最优为两点间距，因此来设定为`h(x)`，一定层度上避免了南辕北辙的节点间距（但有可能是最优的节点路径）  

