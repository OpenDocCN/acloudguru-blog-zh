# 面向初学者的 Linux sudo 命令|云专家

> 原文：<https://acloudguru.com/blog/engineering/linux-commands-for-beginners-sudo>

Sudo，一个统治他们的命令。它代表“超级用户做！”发音像“苏面团”。

作为 Linux 系统管理员或高级用户，这是您的武器库中最重要的命令之一。你有没有试过在终端中运行一个命令却得到“拒绝访问”的回答。这是给你的命令！但是，权力越大，责任越大！运行 sudo 命令比作为 root 用户登录，或者使用 su 的“切换用户”命令要好得多。请继续阅读，看看 sudo 能为您做些什么！

* * *

## 加速您的职业发展

[从 ACG 开始](https://acloudguru.com/pricing)通过 AWS、Microsoft Azure、Google Cloud 等领域的课程和实际动手实验室改变你的职业生涯。

sudo 是干什么用的？

* * *

## 那么，sudo 是用来做什么的呢？如果在任何 Linux 命令前加上前缀“sudo ”,它将以提升的权限运行该命令。执行某些管理任务需要提升权限。有一天你可能希望运行 LAMP (Linu Apache MySQL PHP)服务器，并且必须手动编辑你的配置文件。您可能还需要重启或重置 Apache web 服务器或其他服务守护进程。您甚至需要提升特权来关闭或重启计算机。“嘿，谁把这东西关了？!"如果你熟悉 Windows，它与你试图做任何重要事情时弹出的 Windows 用户帐户控制对话框非常相似，只是不那么友好。

在 Windows 中，如果您尝试执行管理任务，会出现一个对话框询问您是否希望继续(“您真的确定要运行刚才单击的程序吗？”).然后执行任务。在 Mac 上，会弹出一个安全对话框，要求您输入密码并单击确定。在 Linux 中，这更像是一个戏剧性的故事。没有适当的权限，事情可能会表现得很奇怪。您正在编辑的重要配置文件可能无法正确保存。您安装的程序可能会拒绝运行。你下载的那个很棒的源代码需要编译。你甚至可能幸运地得到一个“拒绝访问”或另一个友好的错误信息。所有你最害怕的事情都变成了现实，但是你需要做的就是请求许可！这就是为什么我们要记住像这样提前请求超级用户权限:

如果我们不首先提升 sudo 的权限，看看这个截图会发生什么。首先，我们使用 reboot 命令尝试重启系统。该命令失败的原因是:“必须是超级用户”。然后我们尝试用 *sudo* 重启。Sudo 会询问您的用户密码。请注意，它要求您输入密码，而不是 root 密码。最后，我们看到广播消息，系统现在将重新启动。

```
sudo reboot
```

须藤就像说了一个神奇的词。它也可以被命名为 opensesame 或 abracadabra，甚至 bippityboppitybacon。

****为什么 sudo 比替代品更好？****

### Sudo 是提升特权的最好也是最安全的方式。让我们来看看另一种做事方式。交换机用户命令“su”将要求您输入 root 密码，并给出一个超级用户提示，用#符号表示。那个#符号的意思是“危险！您以 ROOT 用户身份登录！”。你发出的第一个命令可能会很顺利。但是您的健忘会导致您以 root 用户身份登录。一个错误的打印然后砰！你删除了整个硬盘，而不是你下载的那个假 mp3。这只猫决定躺在你温暖的笔记本电脑上。噗！你的网络服务器和家庭业务都没了！

使用 sudo 命令，您必须在每个命令之前输入“sudo”。这意味着你不必记得切换回常规用户模式，事故会更少。

****苏多斯文件****

### 这份文件是须藤的阴暗面。它控制谁可以使用 sudo 命令获得提升的权限。它通常位于/etc/sudoers。编辑该文件的最佳和最安全的方法是使用 visudo 命令。该命令将以提升的权限启动 vi 编辑器，以便您可以编辑并保存文件。它还会在 sudoers 文件上加一个文件锁，这样其他人就不能编辑它了。

编辑完成后，它会分析文件中的简单错误。这是编辑 sudo 文件的一种更安全的方式，而不是仅仅使用任何旧的文本编辑器。该文件包含许多参数。您可以指定哪些组的哪些用户可以执行哪些命令。我们只是通过在底部添加以下内容来授予自己对 sudo 的访问权限:

现在，指定的用户名将能够使用所有 root 权限。您还可以允许用户或组只对特定的服务或服务器进行 sudo 访问，以代替 ALL 参数，但这是另一天的主题。

```
username   ALL=(ALL)       ALL //gives user "username" sudo access%wheel     ALL=(ALL)       ALL //Gives all users that belong to the wheel group sudo access
```

****如何用 sudo 做更多事？****

### 像任何好的命令一样，有一些漂亮的选项可以让 sudo 做得更多！*sudo–b*将在后台运行该命令。这对于运行时显示大量输出的命令非常有用。*sudo–s*将使用提升的权限运行指定的 shell，并给出#提示符(不要忘记退出！).并且*sudo su–*将使您成为根用户并加载您的自定义用户环境变量。

**使用 Linux sudo 命令**

### 当我们想要运行重要的命令时，Sudo 给了我们安全的特权。它可能是 Ubuntu 用户中使用最多、最强大的命令，因为它已经成为该发行版中的首选方法。现在你有了权力，在发布命令的时候一定要确保安全！没有 su-undo！

如果你准备好让你的学习更上一层楼，请查看我们的[Linux 概述](https://acloudguru.com/course/overview-of-linux)课程。

提升您的云计算职业生涯

* * *

### 无论您是云新手还是专家，云专家都能让您轻松(而且非常棒)地获得认证并掌握现代技术技能。查看我们当前的 [**免费云课程**](https://acloudguru.com/blog/news/whats-free-at-acg) 或通过免费试用提升您的 [**云和 it 职业道路**](https://acloudguru.com/platform/training-paths) 。

其他 Linux 命令行资源:

* * *

### Other Linux Command Line Resources: