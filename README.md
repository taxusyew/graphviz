graphviz
========

练习graphviz创建关系图

开头digraph <文件名> { <body\> }

设定图片大小：   
				
				size="@, @"

直接写变量a，b，main，init...都会变成节点中的文字

修改连接线样式： 

				main->init[style=dotted];  // 设定为虚线

修改node样式：  

			   c[sharp=polygon, sides =4, color=lightblue, style=filled];
			   c[shape=box]  // 由默认的椭圆，变为方块

修改node结构：
			
			   node[label ="<f0> | <f1> G | <f2> "];  // 三列一行的表，表示树中的叶子节点
			   "node0": f2->"node4":f1;     // node0中的f2列指向node4中的f1列
子图：

			   subgraph <图id> {}