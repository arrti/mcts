# mcts
An Python N-in-Row game based on Monte Carlo Tree Search and UCT RAVE.    
一个Python实现的使用蒙特卡洛搜索树（MCTS）和UCT RAVE的"N-in-Row"类游戏。

## 2017.2.23 更新
１．`n_in_row_not_so_correct.py`其实并未能完全正确的实现MCTS，因为它单位时间内模拟的次数多，根据MC的原理，所以它的表现也没有那么差，但它依旧是不正确的；        
２．`n_in_row_uct_rave_not_so_correct.py`在上面的基础上进一步实现了UCT RAVE；          
３．`n_in_row_uct_rave.py`则是在阅读了论文《Monte-Carlo tree search and rapid action value estimation in computer Go》后实现的正确的版本——也许吧，欢迎与我一起讨论。            

具体的说明已经更新到了[博客](http://www.cnblogs.com/xmwd/p/python_game_based_on_MCTS_and_UCT_RAVE.html)。  
**注意：** 需要使用Python3运行上面的代码。

## TODO
因为`n_in_row_uct_rave.py`中需要遍历的节点激增，单位时间内模拟的次数较少，所以短时间（少于15s）模拟的表现上不如之前的“错误”的算法，考虑通过多线程等手段来进一步提高单位时间内的模拟次数。

