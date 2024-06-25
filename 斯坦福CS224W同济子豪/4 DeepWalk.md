## Word2vec
word2vec 的假设：相邻单词应该相似
在 man 和 woman 是平行的，king 和 queen 也是平行的。

![800](4%20DeepWalk/image-20240624200843004.png)

通过构造下面这两个自监督任务，得到词向量。

![800](4%20DeepWalk/image-20240624201105438.png)

## DeepWalk
一个醉汉随机在图上走，他所走的路径就是一句话，每个节点就是一个单词

为了把每一个节点编码成一个向量：

![](4%20DeepWalk/image-20240624201513569.png)

在 Deepwalk 里面，采用机器学习的方式来完成这种降维处理（原来的邻接矩阵只有 0 和 1 两个取值，而 Latent Dimensions 每个值可以有很多的取值） 
 
![](4%20DeepWalk/image-20240624201749085.png)

