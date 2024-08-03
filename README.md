# [黑客的贝叶斯方法](http://camdavidsonpilon.github.io/Probabilistic-Programming-and-Bayesian-Methods-for-Hackers/)
#### *使用Python和PyMC*

贝叶斯方法是推理的自然方法，但它被慢慢的数学分析章节隐藏起来。关于贝叶斯推理的典型文本包括两到三章的概率论，然后介绍贝叶斯推理是什么。不幸的是，由于大多数贝叶斯模型的数学难解性，读者只能看到简单的、人工的例子。这会让用户对贝叶斯推理产生“然后呢”的感觉。事实上，这也是作者之前的看法。

在贝叶斯方法在机器学习竞赛中取得一些成功后，我决定再次研究这个主题。即使有我的数学背景，我也花了三天时间阅读例子并试图拼凑出这些方法。文献中缺乏将理论与实践联系起来的内容。我误解的问题在于贝叶斯数学与概率编程之间的脱节。话虽如此，我当时的痛苦就是为了让读者现在不必再受苦。这本书试图弥合这个差距。

如果贝叶斯推理是目的地，那么数学分析是一条特定的路径。而另一方面，计算能力已经足够便宜，我们可以通过概率编程走另一条路线。后者路径更有用，因为它否定了每一步都需要数学干预的必要性，也就是说，我们取消了贝叶斯推理前常常难以处理的数学分析。简单来说，后者的计算路径通过从头到尾的小中间跳跃来进行，而第一条路径则通过巨大的飞跃，往往远离我们的目标。此外，没有强大的数学背景，第一条路径所需的分析甚至无法进行。

*黑客的贝叶斯方法*被设计为从计算/理解优先，数学次之的角度介绍贝叶斯推理。当然，作为一本入门书，我们只能停留在此：一本入门书。对于有数学背景的人，他们可以用其他以数学分析为目的的书籍来满足这本书产生的好奇心。对于数学背景较少的爱好者，或者对数学不感兴趣但对贝叶斯方法的实践感兴趣的人，这本书应该是足够且有趣的。

选择PyMC作为概率编程语言有两个原因。截至本文撰写时，PyMC领域还没有一个中心资源来提供示例和解释。官方文档假定先前了解贝叶斯推理和概率编程。我们希望这本书能鼓励各个层次的用户关注PyMC。其次，随着Python科学栈的最新核心开发和普及，PyMC很可能很快成为核心组件。

PyMC运行有一些依赖项，主要是NumPy和（可选的）SciPy。为了不限制用户，本书中的例子将仅依赖PyMC、NumPy、SciPy和Matplotlib。

由Addison-Wesley出版的印刷版
------
<div style="float: right; margin-left: 30px;"><img title="Bayesian Methods for Hackersg" style="float: right;margin-left: 30px;" src="http://www-fp.pearsonhighered.com/assets/hip/images/bigcovers/0133902838.jpg" align=right height = 200 /></div>

**《黑客的贝叶斯方法》现在有印刷版了！** 你可以在[亚马逊](http://www.amazon.com/Bayesian-Methods-Hackers-Probabilistic-Addison-Wesley/dp/0133902838)上购买一本。在线版本和印刷版本有什么区别？

 - 额外的贝叶斯A/B测试章节
 - 更新的示例
 - 章末问题的答案
 - 额外的解释和重新编写的部分，以帮助读者。

目录
------

请参阅项目主页[这里](http://camdavidsonpilon.github.io/Probabilistic-Programming-and-Bayesian-Methods-for-Hackers/)以获取示例。

以下章节通过 *nbviewer* 在[nbviewer.jupyter.org/](http://nbviewer.jupyter.org/)渲染，只读并实时渲染。
可以通过克隆下载交互式笔记本和示例！

### PyMC2

* [**前言:**](http://nbviewer.jupyter.org/urls/raw.github.com/CamDavidsonPilon/Probabilistic-Programming-and-Bayesian-Methods-for-Hackers/master/Prologue/Prologue.ipynb) 为什么我们要做这件事。

* [**第1章：贝叶斯方法简介**](http://nbviewer.jupyter.org/urls/raw.github.com/CamDavidsonPilon/Probabilistic-Programming-and-Bayesian-Methods-for-Hackers/master/Chapter1_Introduction/Ch1_Introduction_PyMC2.ipynb)
    介绍贝叶斯方法的哲学和实践，并回答“什么是概率编程？”的问题。示例包括：
    - 推断人类行为变化的短信率

* [**第2章：更多关于PyMC的内容**](http://nbviewer.jupyter.org/urls/raw.github.com/CamDavidsonPilon/Probabilistic-Programming-and-Bayesian-Methods-for-Hackers/master/Chapter2_MorePyMC/Ch2_MorePyMC_PyMC2.ipynb)
    通过示例探索使用Python的PyMC库建模贝叶斯问题。我们如何创建贝叶斯模型？示例包括：
    - 在避免撒谎者的情况下检测作弊学生的频率
    - 计算挑战者航天飞机灾难的概率

* [**第3章：打开MCMC的黑箱**](http://nbviewer.jupyter.org/urls/raw.github.com/CamDavidsonPilon/Probabilistic-Programming-and-Bayesian-Methods-for-Hackers/master/Chapter3_MCMC/Ch3_IntroMCMC_PyMC2.ipynb)
    我们讨论MCMC的操作和诊断工具。示例包括：
    - 使用混合模型进行贝叶斯聚类

* [**第4章：从未讲述的最伟大的定理**](http://nbviewer.jupyter.org/urls/raw.github.com/CamDavidsonPilon/Probabilistic-Programming-and-Bayesian-Methods-for-Hackers/master/Chapter4_TheGreatestTheoremNeverTold/Ch4_LawOfLargeNumbers_PyMC2.ipynb)
    我们探索一个非常有用且危险的定理：大数法则。示例包括：
    - 探索Kaggle数据集和天真的分析陷阱
    - 如何按好坏顺序对Reddit评论进行排序（不像你想象的那么容易）

* [**第5章：你宁愿失去一只胳膊还是一条腿？**](http://nbviewer.jupyter.org/urls/raw.github.com/CamDavidsonPilon/Probabilistic-Programming-and-Bayesian-Methods-for-Hackers/master/Chapter5_LossFunctions/Ch5_LossFunctions_PyMC2.ipynb)
    介绍损失函数及其在贝叶斯方法中的（精彩）使用。示例包括：
    - 解决《价格合适》中的对决
    - 优化财务预测
    - Kaggle黑暗世界竞赛的获胜解决方案

* [**第6章：将我们的“先验”-择优放在首位**](http://nbviewer.jupyter.org/urls/raw.github.com/CamDavidsonPilon/Probabilistic-Programming-and-Bayesian-Methods-for-Hackers/master/Chapter6_Priorities/Ch6_Priors_PyMC2.ipynb)
    可能是最重要的一章。我们借助专家意见回答问题。示例包括：
    - 多臂强盗和贝叶斯强盗解决方案。
    - 数据样本大小与先验之间的关系是什么？
    - 使用专家先验估计财务未知数

    我们探索在分析中保持客观的有用提示以及先验的常见陷阱。

### PyMC3

* [**前言:**](http://nbviewer.jupyter.org/urls/raw.github.com/CamDavidsonPilon/Probabilistic-Programming-and-Bayesian-Methods-for-Hackers/master/Prologue/Prologue.ipynb) 为什么我们要做这件事。

* [**第1章：贝叶斯方法简介**](http://nbviewer.jupyter.org/urls/raw.github.com/CamDavidsonPilon/Probabilistic-Programming-and-Bayesian-Methods-for-Hackers/master/Chapter1_Introduction/Ch1_Introduction_PyMC3.ipynb)
    介绍贝叶斯方法的哲学和实践，并回答“什么是概率编程？”的问题。示例包括：
    - 推断人类行为变化的短信率

* [**第2章：更多关于PyMC的内容**](http://nbviewer.jupyter.org/urls/raw.github.com/CamDavidsonPilon/Probabilistic-Programming-and-Bayesian-Methods-for-Hackers/master/Chapter2_MorePyMC/Ch2_MorePyMC_PyMC3.ipynb)
    通过示例探索使用Python的PyMC库建模贝叶斯问题。我们如何创建贝叶斯模型？示例包括：
- 在避免撒谎者的情况下检测作弊学生的频率
- 计算挑战者航天飞机灾难的概率
* [**第3章：打开MCMC的黑箱**](http://nbviewer.jupyter.org/urls/raw.github.com/CamDavidsonPilon/Probabilistic-Programming-and-Bayesian-Methods-for-Hackers/master/Chapter3_MCMC/Ch3_IntroMCMC_PyMC3.ipynb)
    我们讨论MCMC的操作和诊断工具。示例包括：
    - 使用混合模型进行贝叶斯聚类

* [**第4章：从未讲述的最伟大的定理**](http://nbviewer.jupyter.org/urls/raw.github.com/CamDavidsonPilon/Probabilistic-Programming-and-Bayesian-Methods-for-Hackers/master/Chapter4_TheGreatestTheoremNeverTold/Ch4_LawOfLargeNumbers_PyMC3.ipynb)
    我们探索一个非常有用且危险的定理：大数法则。示例包括：
    - 探索Kaggle数据集和天真的分析陷阱
    - 如何按好坏顺序对Reddit评论进行排序（不像你想象的那么容易）

* [**第5章：你宁愿失去一只胳膊还是一条腿？**](http://nbviewer.jupyter.org/urls/raw.github.com/CamDavidsonPilon/Probabilistic-Programming-and-Bayesian-Methods-for-Hackers/master/Chapter5_LossFunctions/Ch5_LossFunctions_PyMC3.ipynb)
    介绍损失函数及其在贝叶斯方法中的（精彩）使用。示例包括：
    - 解决《价格合适》中的对决
    - 优化财务预测
    - Kaggle黑暗世界竞赛的获胜解决方案

* [**第6章：将我们的“先验”-择优放在首位**](http://nbviewer.jupyter.org/urls/raw.github.com/CamDavidsonPilon/Probabilistic-Programming-and-Bayesian-Methods-for-Hackers/master/Chapter6_Priorities/Ch6_Priors_PyMC3.ipynb)
    可能是最重要的一章。我们借助专家意见回答问题。示例包括：
    - 多臂强盗和贝叶斯强盗解决方案。
    - 数据样本大小与先验之间的关系是什么？
    - 使用专家先验估计财务未知数

    我们探索在分析中保持客观的有用提示以及先验的常见陷阱。

**关于PyMC的更多问题？**
请在[交叉验证](http://stats.stackexchange.com/)上发布您的建模、收敛或任何其他PyMC问题。

使用本书
-------

本书可以通过三种不同方式阅读，从最推荐到最不推荐：

1. 最推荐的选项是克隆存储库以将.ipynb文件下载到本地计算机。如果您安装了Jupyter，可以在浏览器中查看章节*并*编辑和运行提供的代码（并尝试一些练习问题）。这是阅读本书的首选选项，尽管它有一些依赖项。
    -  Jupyter是查看ipynb文件的必需品。可以在[这里](http://jupyter.org/)下载。Jupyter笔记本可以通过`(your-virtualenv) ~/path/to/the/book/Chapter1_Introduction $ jupyter notebook`运行
    -  对于Linux用户，安装NumPy、SciPy、Matplotlib和PyMC应该没有问题。对于Windows用户，如果遇到困难，请查看[预编译版本](http://www.lfd.uci.edu/~gohlke/pythonlibs/)。
    -  在styles/目录中有许多文件（.matplotlirc），用于使事情变得漂亮。这些不仅为本书设计，还提供了许多默认设置的改进。
2. 第二个首选选项是使用nbviewer.jupyter.org网站，在浏览器中显示Jupyter笔记本（[示例](http://nbviewer.jupyter.org/urls/raw.github.com/CamDavidsonPilon/Probabilistic-Programming-and-Bayesian-Methods-for-Hackers/master/Chapter1_Introduction/Ch1_Introduction_PyMC2.ipynb)）。
内容会随着书的提交而同步更新。您可以使用上面的目录部分链接到章节。

3. PDF是阅读本书的最不推荐方法，因为PDF是静态且不可交互的。如果需要PDF，可以使用[nbconvert](https://github.com/jupyter/nbconvert)工具动态创建。

安装和配置
------

如果您想在本地运行Jupyter笔记本（上述选项1），您需要安装以下内容：

-  Jupyter是查看ipynb文件的必需品。可以在[这里](http://jupyter.org/install.html)下载
- 必要的软件包是PyMC、NumPy、SciPy和Matplotlib。
   -  对于Linux/OSX用户，安装上述软件包应该没有问题，[*除了OSX上的Matplotlib*](http://www.penandpants.com/2012/02/24/install-python/)。
   -  对于Windows用户，如果遇到困难，请查看[预编译版本](http://www.lfd.uci.edu/~gohlke/pythonlibs/)。
   - 还推荐用于数据挖掘练习的[PRAW](https://github.com/praw-dev/praw)和[requests](https://github.com/kennethreitz/requests)。
- 新手Python或Jupyter，需要帮助理解命名空间？请查看[这个回答](http://stackoverflow.com/questions/12987624/confusion-between-numpy-scipy-matplotlib-and-pylab)。

-  styles/目录中有许多为笔记本自定义的文件。
这些不仅为本书设计，还提供了许多默认设置的改进。
笔记本中的样式尚未最终确定。

开发
------

本书有一个不寻常的开发设计。内容是开源的，这意味着任何人都可以成为作者。
作者使用GitHub界面提交内容或修订。

### 如何贡献

#### 贡献什么？

-  当前的章节列表尚未确定。如果您发现缺少的内容（MCMC、MAP、贝叶斯网络、好的先验选择、潜在类等），
请从那里开始。
-  清理Python代码并使代码更符合PyMC风格
-  提供更好的解释
-  拼写/语法错误
-  建议
-  为Jupyter笔记本样式做出贡献

#### 提交

-  所有提交都是欢迎的，即使它们是微小的;)
-  如果您不熟悉GitHub，可以通过以下电子邮件发送贡献。

评论
------
*这些是讽刺性的，但是真实的*

“不，但看起来不错” - [John D. Cook](https://twitter.com/JohnDCook/status/359672133695184896)

“我...读了这本书...我喜欢它！” - [Andrew Gelman](http://www.andrewgelman.com/2013/07/21/bayes-related)

“这本书是一份福音，是对‘嗯哼！你不懂数学，滚开！’这种思想的直接反驳...
出版模式非常不寻常。不仅是开源的，而且依赖于任何人的拉取请求来推进这本书。这是非常聪明和鼓舞人心的。” - [兴奋的Reddit用户](http://www.reddit.com/r/Python/comments/1alnal/probabilistic_programming_and_bayesian_methods/)