# 算法偏差:它是什么，如何处理？|云专家

> 原文：<https://acloudguru.com/blog/engineering/algorithmic-bias-explained>

在这篇文章中，我分解了什么是算法偏差，它如何在机器学习系统中出现，以及如何减轻它。我将更详细地介绍不同类型的偏见以及偏见的负面商业影响。

如果你对亚马逊网络服务(AWS)提供的工具感兴趣，这些工具可以通过检测潜在的偏见来帮助改善你的机器学习模型，我也会为你提供帮助。

## **什么是算法偏差？**

机器学习算法是分析复杂数据集以揭示趋势和模式的计算机程序。每种算法都代表了机器在数据中寻找意义的一步一步的指令。有许多算法(例如，分类、聚类、回归、异常检测等等)通常按照所使用的机器学习技术来分组:监督学习、非监督学习、强化学习等等。

这些算法将趋势和模式存储在他们的发现的数学表示中，称为机器学习模型(或简称为模型)。一旦模型被训练来识别模式，就可以向它提供以前从未见过的数据来进行分析、分类和提出建议。

机器不是人类，从理论上讲，不应该被人类的偏见和偏向所引导——那么，一台机器怎么会表现出算法偏向(或者仅仅是偏向)？一个算法怎么会产生一个模型，因为偏差而做出不公平的预测和推荐呢？我们先退一步来探讨一下当今世界上机器学习的使用情况。

企业和许多联邦组织使用机器学习来分析数据，以回答人类无法人工分析的复杂问题。今天，模型根据研究数据提出建议和预测，称为推论。对人进行推断，包括他们的身份、人口属性、偏好和可能的未来行为。甚至可以对一个人的健康做出推断！

从伦理的角度来看，推论应该是公平的，尤其是那些预测一个人的偏好和可能的未来行为的推论。当推论系统地对来自特定群体的个体不太有利时，算法偏差就出现了，在特定群体中，群体之间没有相关的差异来证明推荐是正确的。有偏见的推荐常常通过拒绝给予他人某些机会来剥夺人们的权利。

## 算法偏差的真实例子是什么？

让我们来挖掘一些机器学习中算法偏差的实际例子。

对于咖啡因上瘾者来说，没有一杯温暖的优质烘焙咖啡、一杯冰焦糖星冰乐或一杯热茶拿铁就无法开始新的一天，有时你不知道接下来该尝试什么。一个伟大的商业策略是使用机器学习，特别是强化学习，来提供产品推荐，使客户的偏好保持在脑海中，同时介绍客户可能喜欢的新产品。

假设开发了一个推荐引擎，它从数据中了解到 20 岁以下的客户更喜欢星冰乐而不是浓缩咖啡饮料。有了这个新发现的知识，推荐引擎再也不会向 20 岁以上的顾客推荐当季的新口味，南瓜香料！可以认为推荐引擎对 20 岁以上的人有偏见。

错误地推荐(或不推荐)一种饮料听起来也没那么糟糕，对吧？一个 20 岁以上的人错过了新一季的味道并不是世界末日！你有没有考虑过，当用于训练饮料推荐引擎的相同实践和技术被转移到企业的其他部分，如招聘或雇用时，会发生什么？

想象一下，一个由机器学习驱动的招聘工具用于审查求职者的简历，以自动化和加速搜索顶级软件工程人才。在这种情况下使用机器学习可以审查 1000 份简历，并快速确定要聘用的前 10 名。

嗯，这个招聘工具不是想象出来的；该工具是由一家知名公司开发的，并在招聘中使用了几年。然而不幸的是，这个工具被发现对女性有偏见。它最终被关闭了，因为它降级了包含“女性”一词的简历，如“技术领域的女性”或“编码女性”。它还惩罚了来自女子大学的简历。

招聘工具了解到，通过观察以前提交的软件工程职位简历中的模式，男性可以成为更好的软件工程师。大多数简历来自男性，这反映了男性在整个科技行业的主导地位。这种不受约束的偏见产生了不必要的影响，因为它延续了技术领域已经存在的不平等。

## 偏见对企业有什么负面影响？

在前机器学习世界，人类做出招聘、广告、贷款和刑事判决决定。这些决策受联邦、州和地方法律管辖，这些法律规定了公平、透明和公正的决策过程。现在，机器要么做出这些决定，要么严重影响这些决定。最重要的是，保护和执行发明创造者和所有者权利的知识产权(IP)法律保护算法决策过程的输入。

算法偏差有许多负面影响:

*   不公平地分配机会、资源或信息
*   侵犯公民自由
*   让个人的安全受到质疑
*   未能向某些人提供与其他人相同的服务质量
*   对个人福祉的负面影响，如被认为是贬损或冒犯的经历
*   内部冲突和员工对更多道德实践的需求

## 线上有什么？

有偏见的决策会对组织的声誉、消费者的信任以及未来的业务和市场机会产生负面影响。今天，政府正在为算法决策制定法规和立法。没有将解决机器学习中的偏见作为优先事项的组织可能会在未来的某个时候受到处罚和高额罚款。

组织应该现在就开始促进机器学习中的道德和责任文化，以免为时过晚，并利用他们的声音推动行业变革和负责任的人工智能实践的监管。机器学习系统的开发者应该标记伦理问题，并认识到他们在开发机器学习系统时所承担的道德和伦理责任。

## 偏见在机器学习系统中是如何呈现的？

偏见在机器学习系统中有许多表现方式。通常情况下，由算法研究以确定趋势和模式的数据集是罪魁祸首。在机器学习招聘工具的例子中，该算法研究了 10 年以前提交的简历。It 专业的男性大多会为软件工程职位投简历；因此，从数学上讲，男性可能会成为更好的软件工程师。

你不能责怪机器，但你可以责怪向机器提供数据的开发人员。提供的数据集不均衡，导致有偏见的决策。

以下是我们将涉及的三种不同类型的数据相关偏差的快速总结:

*   **采样偏差:**收集的数据不能反映解决方案将运行的环境，从而导致偏差。
*   **排除偏差:**不适当地删除数据点或记录的行为，因为它们被认为是不相关的，从而导致偏差。
*   **观察者偏差:**记录数据的观察者看到了他们期望或想要看到的东西，这导致他们错误地标注了数据。

### 抽样偏误

采样偏差发生在机器学习生命周期的数据收集阶段。回到招聘工具的例子，样本数据集包含的男性简历多于女性，导致推荐倾向于男性。这是抽样偏差的一个典型例子:收集的数据并不代表工具运行的环境，因为申请软件工程职位的男性和女性数量相等。

### 排斥偏差

排除偏差通常发生在机器学习生命周期的数据准备阶段，通常从数据集中排除一些特征(即数据点)，通常在清理和准备数据的保护伞下。

让我们以一个机器学习驱动的预测引擎为例，该引擎用于预测一种新的星冰乐在午餐时间的受欢迎程度(在全球范围内)。这种系统通常用于在新产品上市时帮助预测收入和营销决策。将由机器学习算法分析的数据集包括过去在午餐高峰期间购买的类似星冰乐。

在查看数据集时，开发人员注意到下午 2 点到 4 点有星冰乐购买。开发人员删除了那些错误的记录(或观察)，因为典型的午餐时间是从上午 11:30 到下午 2 点。开发商没有意识到西班牙的午餐时间往往是从下午 2 点到 3 点，而西班牙的午休时间是从下午 2 点到 5 点，这影响了人们吃午餐的时间。

在这种情况下，开发人员删除了记录，认为它们是基于他们预先存在的信念不相关的，导致系统偏向于美国的午餐时间。

预测引擎继承了开发者的信念和偏见。当您有数 Pb 或更多的数据时，很容易选择一个小样本来进行训练，但是您可能会无意中排除重要的数据，从而导致偏差。

### 观察者偏差

观察者偏差，有时也称为确认偏差，通常发生在机器学习生命周期的数据标记阶段，由观察者记录他们希望或期望在数据中看到的内容而产生。

让我们以在提供的图像中识别星冰乐味道的图像分类系统为例。该算法分析的数据集包括许多标有风味名称的星冰乐图像。有人首先必须标记(或识别)每个图像中显示的饮料风味，这是一个非常手工的过程。

想象一下，负责标记图像的观察者倾向于将焦糖可可簇风味误标为肉桂卷，仅仅因为肉桂卷是他们最喜欢的风味。在这种情况下，他们在数据中看到他们想要的东西。这种手动贴标过程容易出现人为错误，导致模型错误地识别口味，并偏向肉桂卷星冰乐。

虽然还有许多其他类型的偏差，但这三种是由数据引起的最普遍的偏差。现在你已经了解了偏见，让我们来探索减少偏见的方法。

## **如何减轻偏见？**

减轻采样、排除或观察者偏差的最佳方法是在将数据交给算法进行分析之前，实践负责任的数据集开发。

### 减轻采样偏差

为了减轻采样偏差，请确保为您的模型将要遇到的所有情况收集数据。确保公平的班级代表性和在训练前平均分配数据对减少偏差大有帮助。一些奇特的技术可以修复不平衡的数据集，如过采样和欠采样。SMOTE(合成少数过采样技术)是另一种允许您生成合成数据来解决问题的技术。

### 减轻排斥偏见

为了减少排除偏差，在移除特征和观察值之前，要对它们进行充分的分析。此外，在删除数据之前，看看你自己的偏见。有一些技术可以帮助您进行分析，并帮助您计算要素的重要性:

*   **检查每个特征的系数得分:**这是分配给每个输入值的数字，用于确定该特征的重要程度；数字越高，对推荐或预测的影响越大。
*   **使用可用于基于树的模型的 feature_importances 属性:**在训练任何基于树的模型(即 XGBoost)后，通过绘制条形图直观地检查特性的重要性。
*   **使用主成分分析(PCA)得分:**这是众所周知的降维方法，但也可用于确定特征重要性。

### 减轻观察者的偏见

为了减少排除偏差，确保做数据标记的观察者受过良好的训练，并对潜在偏差进行筛选。这需要了解你的数据，并训练观察者注意什么。

AWS 不仅提供工具来管理机器学习系统的端到端生命周期，还提供工具来帮助检测偏差。 [Amazon SageMaker Clarify](https://aws.amazon.com/sagemaker/clarify/) 是一款工具，通过检测和减轻数据集和模型中的偏差，扩展了 [Amazon SageMaker](https://aws.amazon.com/sagemaker/) 的功能。该工具允许您在机器学习模型开发过程的每个阶段评估偏差-在数据分析、训练和推理期间。当[这款工具在 AWS re:Invent 2020](https://acloudguru.com/blog/engineering/sagemaker-clarify-is-the-most-important-reinvent-announcement-of-the-year) 发布时，我非常兴奋。

随着机器学习从研究实验室走向企业，算法偏差是充分实现机器学习好处的巨大障碍。我们已经看到，当收集和准备数据时，偏差会影响最终模型，从而导致不准确和歧视性的预测。

如果您意识到数据中的偏差，可以实施经过验证的缓解策略。AWS 甚至提供工具来帮助检测和减轻数据集和训练模型中的偏差。

作为开发人员，我们有责任确保我们正在实践负责任的数据集开发，并防止偏见进入生产。

#### 关于作者

[*凯莎·威廉姆斯*](https://twitter.com/keshawillz) *是一位屡获殊荣的技术领导者。她还是 AWS 机器学习英雄、HackerRank 全明星和 Alexa 冠军。*

* * *

## 了解有关机器学习的更多信息

一位云专家提供了一条关于 AWS 机器学习的[专用学习路径](https://acloudguru.com/learning-paths/aws-machine-learning)。无论你处于机器学习之旅的哪个阶段——从新手到经验丰富的专业人士——我们都有课程让你更上一层楼。除了观看视频，您还可以通过动手实验室获得实践经验，并有机会获得多项行业认可的 AWS 认证。

您还可以访问 Pluralsight 广泛的[机器学习路径和课程](https://www.pluralsight.com/browse/machine-learning)。在你自己的时间里，向拥有机器学习实际经验的专家学习。