

# 20180720-20180726
## 周待做列表
* 将clock代码封装成一个class，给冯新宇提供接口；
* 改步态识别的代码，搭建系统；
* 看自然语言处理的一些东西，了解什么叫词向量等。
## clock class封装
>参考：https://blog.csdn.net/dfdfdsfdfdfdf/article/details/52439651
>>vector作为参数的三种传参方式：https://www.cnblogs.com/xiaoxi666/p/6843211.html
## 改步态识别的代码
>要拍摄视频<br>
买三脚架<br>
得到步宽信息<br>
尝试正面视频的处理<br>
## 自然语言处理
### 词嵌入、词向量（word embedding、word vector）
参考：[词嵌入](https://blog.csdn.net/ch1209498273/article/details/78323478)<br>
词嵌入是将词汇映射到实数向量的方法总称。将文本X{x1,x2,x3,x4,x5……xn}映射到多维向量空间Y{y1,y2,y3,y4,y5……yn }，这个映射的过程就叫做词嵌入。  
#### 词嵌入的三种方法：
>**1.Embedding Layer**<br>
Embedding Layer是与特定自然语言处理上的神经网络模型联合学习的单词嵌入。该嵌入方法将清理好的文本中的单词进行one hot编码（热编码），向量空间的大小或维度被指定为模型的一部分，例如50、100或300维。向量以小的随机数进行初始化。Embedding Layer用于神经网络的前端，并采用反向传播算法进行监督。<br>
>**2.Word2Vec/Doc2Vec**<br>
其核心思想就是基于上下文，先用向量代表各个词，然后通过一个预测目标函数学习这些向量的参数。Word2Vec 的网络主体是一种单隐层前馈神经网络，网络的输入和输出均为词向量。该算法给出了两种训练模型，CBOW (Continuous Bag-of-Words Model) 和 Skip-gram (Continuous Skip-gram Model)。
>>CBOW将一个词所在的上下文中的词作为输入，而那个词本身作为输出，也就是说，看到一个上下文，希望大概能猜出这个词和它的意思。<br>
>>Skip-gram它的做法是，将一个词所在的上下文中的词作为输出，而那个词本身作为输入，也就是说，给出一个词，希望预测可能出现的上下文的词，2-gram比较常用。
### 论言语发音与感知的互动机制
