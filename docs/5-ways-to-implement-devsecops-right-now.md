# 立即实施 DevSecOps 的 5 种方法

> 原文：<https://acloudguru.com/blog/engineering/5-ways-to-implement-devsecops-right-now>

听说过 DevSecOps 这个术语，但不太确定它是什么意思？本文回答了什么是 DevSecOps 的问题，并介绍了实现 DevSecOps 实践的 5 种方法。您还将学习可以用来防范安全漏洞的 DevSecOps 工具。

* * *

## 加速您的职业发展

[从 ACG 开始](https://acloudguru.com/pricing)通过 AWS、Microsoft Azure、Google Cloud 等领域的课程和实际动手实验室改变你的职业生涯。

* * *

## 什么是 DevSecOps？(还有 DevOps 和 DevSecOps 有什么区别？)

DevOps 是一套结合了软件开发(Dev)和 IT 运营(Ops)的实践。DevOps 的主要目标是缩短软件开发生命周期，提供高质量的持续交付。

DevSecOps 是 DevOps 方法的扩展，强调软件开发生命周期每个阶段的安全性。DevSecOps 的目标是确保从最初设计到最终交付的整个软件开发过程都考虑到安全问题。

实现 DevSecOps 有许多好处，包括提高安全性、降低成本和缩短交付时间。然而，实现 DevSecOps 可能是一个挑战，尤其是对于那些对这个概念不熟悉的组织。一个工程机构如何起步？幸运的是，最低限度的资源投资可以在安全态势中获得回报。

所以，这里有五种方法可以实现 DevSecOps，从现在开始。

## 1.让安全团队参与设计过程

如果你在一个安全团队中，你能做的帮助实现 DevSecOps 的最重要的事情之一就是参与设计过程。这样，您可以确保从一开始就考虑到任何安全问题。反过来，这将有助于避免开发过程中的安全问题。

一个好的安全团队应该易于联系，将自己“推销”给组织内的其他工程团队。减少初始约定的摩擦应该是 DevSecOps 领导层的首要任务，与开发人员建立信任，并定期邀请设计评审。

设计审查是安全专业人员提出可能的安全问题的好方法。安全专家可以发现潜在的危险，并提供减轻危险的建议。设计评审应该尽快进行，最好是在编写任何源代码之前。将接近完成的应用程序提供给安全团队进行审查的遗留模型确保了冗长的手动审查和潜在的高成本重构，安全团队被迫采取被动的姿态。

## 2.将安全性视为使能因素，而不是阻碍因素

实现 DevSecOps 的最大挑战之一是让软件开发人员将安全性视为使能因素，而不是阻碍因素。在许多组织中，安全团队被视为“说不的人”。更糟糕的是，开发人员和运营团队经常需要寻找可行的解决方案，而没有安全团队的进一步指导。毫不奇怪，安全控制经常被忽视或规避。

虽然安全团队识别和降低风险很重要，但他们也应该被视为推动者和产品合作者。它们可以帮助开发人员了解如何构建安全的应用程序，并提供最佳实践方面的指导。

DevOps 有一个宗旨:人>过程>工具；重要的是建立一个拥有正确技能的正确团队，这样软件工程师和安全人员才能协同工作。

DevSecOps 最重要的一个方面是在软件开发生命周期的早期捕捉安全问题。

一旦开发人员签入代码，就该开始扫描潜在的问题了。使用像静态分析和供应链监控这样的工具可以在果实进入运行期之前抓住它，从而大大提高安全性。

扫描容器、依赖项和开源库中已知的漏洞也很重要。近年来，发生了几起高调的软件供应链攻击事件。这些攻击带来的大规模安全后果应该是对任何不关注其软件构建基础的人的可怕警告。

### 扫描源代码中的凭据和敏感值

除了扫描供应链，扫描源代码中的凭证和敏感值也很重要。

一些静态分析工具也提供了凭证扫描功能。因此，确定正确的过程和工具来监控您环境中的代码库以发现可疑的提交是非常重要的。

通过预提交挂钩集成提醒开发人员其代码中存在敏感值，这为开发人员提供了一种简单的补救方法，而无需进行繁琐的工作，即轮换机密或对推送的代码进行更改。

最后，静态应用程序安全测试(SAST)工具可以分析源代码，而不需要实际运行代码。在遗留的开发环境中，这通常是手工完成的，但是 DevSecOps 应该专注于使用自动化工具。静态分析可用于查找代码中的漏洞，如 SQL 注入漏洞、命令注入、溢出和跨站脚本(XSS)漏洞。

尽早关注安全性有助于提供快速反馈，并使开发人员能够拥有他们工作的安全性成果，从而形成持续改进的良性循环。

## 4.尽可能自动化安全结果

持续集成/持续交付(CI/CD)管道是任何 DevOps 实施的基础支柱。管道是有效软件交付功能的基础。它支持的测试和部署自动化对于现代软件环境要求的快速交付节奏至关重要。

作为一种安全工具，CI/CD 管道也不例外。传统上繁琐的手动安全流程，如输入验证、集成测试和行为监控，可以通过自动化集成到 DevOps 生命周期中，为技术和非技术利益相关者提供快速、可见的结果。

高功能的 DevSecOps 团队甚至可以期待自动补救，修复易挂的果实，让工程师自由处理更复杂的安全问题。

在 DevOps 文化是新的，甚至不存在的工程组织中，额外的安全用例应该作为一个强有力的卖点，以获得领导对试点项目的认可。与手动流程相比，自动化可以更好地利用现有员工资源，防止安全工作成为业务 KPI 的瓶颈。

开发运维中的安全工作应该是可测量的，具有可量化的结果，可用于显示安全流程和工具的功效。这些数据可以用来决定未来开发工作的重点。此外，与其他团队分享这些成功有助于在整个公司范围内创建一种更具 DevOps 意识的文化，这只会带来好的事情。

## 5.向左移动，但是继续看右边

即使越来越多的安全工作提前进入开发生命周期(“左移”)，对整个工程组织来说，在监控应用程序的健康和行为方面保持警惕，并保持稳固的运营足迹仍然是至关重要的。

在成熟的 DevOps 文化中，开发、运营和安全之间不应该存在孤岛。每个人都拥有安全性，每个人都共同努力来保护他们所负责的应用程序和系统的安全。但是即使在一个运作良好的团队中，关注生产中发生的事情也是很重要的。仅仅因为某个东西构建得很安全，并不意味着它会一直如此。配置更改、新的依赖关系和代码部署都会带来新的风险，需要降低这些风险。尽管我们都不愿意这么想，但人类还是会犯错。

那么，最简单的方法是什么，以确保新的软件服务将轻松地与公司的监控平台集成？DevOps 和 DevSecOps 人员可以参与早期设计会议，指出围绕库和模块的最佳实践，以便与监控堆栈无缝集成。

DevOps 的强大 DevSecOps 工作还可以实现自动化，以在实时工作负载中强制执行正确的配置和行为，向所有者强调错误配置和潜在的安全问题，他们可以着手修复问题。

## 如何实现 DevSecOps 并提高安全性和软件交付

所以，喜欢 DevSecOps 的想法，但不知道如何开始？与任何变革举措一样，从小处着手通常是产生持久影响的最佳方式。

在整个组织中建立共同的安全责任感是第一步，也是最重要的一步。从那以后，只需要实现支持团队的工具和过程。要提高安全和流程最佳实践技能，请查看我们的 [DevOps](https://acloudguru.com/training-library/devops-training) 和[安全](https://acloudguru.com/training-library/security-training)课程。