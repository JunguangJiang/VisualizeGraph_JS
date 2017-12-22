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
shortestPath中<br>
node补充了type{source代表最短路径的源点，target代表最短路径的终点，inPath代表最短路径上的点，outPath代表不在最短路径上的点﻿} <br>
edge补充了type{shortestPath代表最短路径上的点，﻿outsidePath代表不在最短路径上的边}<br>
<br>
ConnectedComponent中<br>
node和edge都补充了group,区分不同的连通域，注意group不是从0开始编号的，而是任意一个整数，但是保证只有相同连通域的节点或者边的group相同<br>
