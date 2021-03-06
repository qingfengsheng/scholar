# N-gram n元语法

指文本中连续出现的n个语词，n元语法模型是基于(n-1)阶马尔可夫链的一种概率语言模型，通过n个语词出现的概率来推断语句的结构。

当n分别为1、2、3时，又分别称为一元语法（unigram）、二元语法（bigram）与三元语法（trigram）



### 应用

- 机器翻译
- 拼写纠错
- 语音识别
- 音字转换
- 自动文摘
- 问答系统
- ......


基于马尔科夫假设（Markov Assumption）：下一个词的出现仅依赖于它前面的一个或几个词。

那么，我们在面临实际问题时，如何选择依赖词的个数，即n。

- 更大的n：对下一个词出现的约束信息更多，具有更大的辨别力；
- 更小的n：在训练语料库中出现的次数更多，具有更可靠的统计信息，具有更高的可靠性。

理论上，n越大越好，经验上，trigram用的最多，尽管如此，原则上，能用bigram解决，绝不使用trigram。



## 参考链接

- [wiki](https://zh.wikipedia.org/wiki/N%E5%85%83%E8%AF%AD%E6%B3%95)
- [语言模型-CSDN](http://blog.csdn.net/xiaokang06/article/details/17965965)
- 