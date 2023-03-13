# 关于 AWS 的新 EC2 Mac 实例，你需要知道什么

> 原文：<https://acloudguru.com/blog/engineering/what-you-need-to-know-about-awss-new-ec2-mac-instances>

昨晚我睡得很早。今天早上醒来，很快就有了这个反应。

## Mac 来到 EC2

AWS 第一次提供了 Mac EC2 实例类型，而不仅仅是简单的实例！他们发布的这款 Mac mini 系列为您提供了*专用的*实例，具有 12 个 CPU 内核、32 GB 内存、10 Gbps 网络(8 Gbps 到 EBS)、登录到 CloudWatch，以及一系列预安装的工具。

macOS Mojave (10.15.6)和 MAC OS Catalina(10 . 15 . 7)ami 包括 AWS CLI、Xcode 命令行工具、SSM 代理和 Homebrew。

## 这是关于 CI/CD 的

这是在 EC2 上发布的，而不是 WorkSpaces，这应该会给我们提供新 mac1.metal 实例的目标受众的线索:**开发者**。

苹果应用程序的 CI/CD 管道传统上被归入数据中心(有时被称为哈利的桌子)。Linux 和 Windows 管道有成熟多样的云产品可供迁移。在苹果方面，已经有几款产品(你好，MacStadium)已经运营了多年，但这是一个利基市场。从某个方面来说，AWS 正在追赶他们。

平心而论，直到 macOS Big Sur 的许可更新，托管 Mac 才不再是法律上的灰色地带。新加入的“许可开发者服务的租赁”部分允许提供商托管 Mac，但有一些严格的限制:

1)只能用于开发者服务，

2)租期必须至少为*24 小时*

3)承租人必须拥有唯一和排他的控制权(减去供应商的管理职能)，以及

4)承租人必须同意系统上的所有软件协议。

最后一部分有点意译，我建议你在这里通读一下。

## 成本是症结所在

AWS 进军这一领域肯定会引起轰动，但采用的限制因素将是它们的定价。

虽然美国的专用主机标价为每小时 1.083 美元(每秒计费)，听起来还不错，但我们必须提前支付 24 小时的费用(根据苹果的许可协议)，这意味着每个实例将花费 25.99 美元才能打开它，即使只是测试。

试图以 AWS 的规模为 MAC 和 iDevices 开发软件，就像我们习惯于其他平台一样，会变得非常昂贵。他们的竞争产品定价低于其初始产品，与在内部运行的专用软件构建 MAC 的总拥有成本相比，这是一个很难推销的产品。(参见 EC2 专用主机定价[此处](https://aws.amazon.com/ec2/dedicated-hosts/pricing/)。)

尽管如此，这里仍有许多令人兴奋的事情。我们可以访问与我们的 AWS 环境深度集成的 macOS 平台。即使我们现在没有将这些工作负载转移到 AWS，我们知道我们可以，并且我们可以相应地规划未来。

Bryson Tyrrell 是 Jamf 的系统开发工程师，通过在 AWS 上进行无服务器开发来推进 Jamf 云平台。