每一个任务都由三个文件完成，html，js和json。js负责逻辑实现，json存储数据。<br>
color.js中存储颜色常量<br>
minSpanTree：最小生成树<br>
shortestPath：最短路径<br>
ConnectedComponent:连通分量<br>

数据说明：<br>
每个json文件中存储一张图graph=<nodes,edges><br>
nodes中的每个node都有一个名字name（就是它的编号，从0开始）<br>
edges中的每个edge都有源点source,终点target<br>
<br>
minSpanTree中<br>
node补充了degree：节点在最小生成树中的度数<br>
<br>
shortestPath中<br>
node补充了type{source代表最短路径的源点，target代表最短路径的终点，inPath代表最短路径上的点，outPath代表不在最短路径上的点﻿} <br>
edge补充了type{shortestPath代表最短路径上的点，﻿outsidePath代表不在最短路径上的边}<br>
<br>
ConnectedComponent中<br>
node和edge都补充了group,区分不同的连通域，注意group不是从0开始编号的，而是任意一个整数，但是保证只有相同连通域的节点或者边的group相同<br>

目前存在的问题<br>
总体不够美观，已经提供了多个json文件用于测试<br>
minSpanTree<br>
1.生成的图太大，无法显示全部<br>
shortestPath<br>
1.最短路径的显示不够友善，路径被其他边挡住了<br>
2.整个图会不断地游走，不能平衡在显示区的中心<br>
ConnectedComponent<br>
1.不同连通域之间的引力太大，总是互相纠缠在一起<br>

