# 深度学习课程简介
内容是学习吴恩达(Andrew Ng)老师的[deeplearning.ai](https://www.coursera.org/specializations/deep-learning)后的学习笔记，国内免费可以同步参看[网易云课堂中内容](https://mooc.study.163.com/university/deeplearning_ai#/c)，具体笔记内容点[这里](https://gaotingwang.github.io/deep-learning-note/)。

- 在[第一门课](https://github.com/gaotingwang/deep-learning-note/tree/master/markdown/1.%E7%A5%9E%E7%BB%8F%E7%BD%91%E7%BB%9C%E5%92%8C%E6%B7%B1%E5%BA%A6%E5%AD%A6%E4%B9%A0)中，将学习如何建立神经网络（包含一个深度神经网络），以及如何在数据上面训练它们。最后将用一个深度神经网络进行辨认猫。

- 在[第二门课](https://github.com/gaotingwang/deep-learning-note/tree/master/markdown/2.%E6%94%B9%E5%96%84%E6%B7%B1%E5%B1%82%E7%A5%9E%E7%BB%8F%E7%BD%91%E7%BB%9C)中，将进行深度学习方面的实践，学习严密地构建神经网络，如何真正让它表现良好，因此你将要学习超参数调整、正则化、诊断偏差和方差以及一些高级优化算法，比如**Momentum**和**Adam**算法，犹如黑魔法一样根据你建立网络的方式。

- 在[第三门课](https://github.com/gaotingwang/deep-learning-note/tree/master/markdown/3.%E7%BB%93%E6%9E%84%E5%8C%96%E6%9C%BA%E5%99%A8%E5%AD%A6%E4%B9%A0%E9%A1%B9%E7%9B%AE)中，学习如何结构化机器学习工程。事实证明，构建机器学习系统的策略改变了深度学习的错误。举个例子：分割数据的方式，分割成训练集、比较集或改变的验证集，以及测试集合，改变了深度学习的错误。

  所以最好的实践方式是什么呢？你的训练集和测试集来自不同的贡献度在深度学习中的影响很大，那么你应该怎么处理呢？

- 在[第四门课](https://github.com/gaotingwang/deep-learning-note/tree/master/markdown/4.%E5%8D%B7%E7%A7%AF%E7%A5%9E%E7%BB%8F%E7%BD%91%E7%BB%9C)中，将会提到卷积神经网络(**CNN(s)**)，它经常被用于图像领域，将会在第四门课程中学到如何搭建这样的模型。

- 最后在[第五门课](https://github.com/gaotingwang/deep-learning-note/tree/master/markdown/5.%E5%BA%8F%E5%88%97%E6%A8%A1%E5%9E%8B)中，将会学习到序列模型，以及如何将它们应用于自然语言处理，以及其它问题。

  序列模型包括的模型有循环神经网络（**RNN**）、全称是长短期记忆网络（**LSTM**）。将在课程五中了解其中的时期是什么含义，并且有能力应用到自然语言处理（**NLP**）问题。总之将在课程五中学习这些模型，以及能够将它们应用于序列数据。比如说，自然语言就是一个单词序列。你也将能够理解这些模型如何应用到语音识别或者是编曲以及其它问题。


## 深度学习兴起原因

![深度学习算法规模](http://www.ai-start.com/dl2017/images/2b14edfcb21235115fca05879f8d9de2.png)

- 数据规模：过去十年的社会里，我们遇到的很多问题只有相对较少的数据量。传统机器学习算法性能一开始在增加更多数据时会上升，但是一段变化后它的性能就会像一个高原一样。我们经常说规模一直在推动深度学习的进步，这里的规模**除了数据的规模，指的也同时是神经网络的规模**，我们需要一个带有许多隐藏单元的神经网络，也有许多的参数及关联性。事实上如今最可靠的方法来在神经网络上获得更好的性能，往往就是**要么训练一个更大的神经网络，要么投入更多的数据**。
- 计算量：在深度学习萌芽的初期，数据的规模以及计算量，局限在我们对于训练一个特别大的神经网络的能力。现在无论是在CPU还是GPU上面，那都使得我们取得了巨大的进步。
- 算法的创新：一个具体的例子，神经网络方面的一个巨大突破是从**sigmoid**函数转换到一个**ReLU**函数。当**sigmoid**函数的梯度接近零，在实现梯度下降的时候，参数会更新的很慢，所以学习的速率也会变的很慢。**ReLU**函数使得梯度下降（**gradient descent**）的算法运行的更快，这就是一个或许相对比较简单的算法创新的例子。但是根本上算法创新所带来的影响，实际上是对计算带来的优化，所以有很多像这样的例子，我们通过改变算法，使得代码运行的更快，这也使得我们能够训练规模更大的神经网络。
