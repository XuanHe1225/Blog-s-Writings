# [「JOISC 2019 Day3」穿越时空 Bitaro](https://loj.ac/problem/3038)

## 题解：

​	不会处理时间流逝，我去看了一眼题解的图，最重要的转换就是把(X,Y)改成(X,Y-X)这样就不会斜着走了。

​	问题变成二维平面上每个横坐标上只有一块区间是空的，你要求的是你从(A,B)走到(C,D)的最短路，直接上线段树维护区间答案和状态。

​	大概就是一段区间，要么它最后等价于一个(L,R)，L是这段区间L的最大值，R是最小值；要么它最后被压成唯一一条路径。

​	代码不想放了，想要的话上loj看吧。