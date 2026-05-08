---
doc_type: web-clipping
url: 'https://catcoding.me/p/weekly-14/'
title: '第 14 期，找出人生中真正重要的事；PowerShell 的故事；好玩的个人主页'
author: 'CatCoding'
site: 'CatCoding'
clipped_at: '2026-05-08T01:46:08.575Z'
source: 'github-web-annotator'
---
# 第 14 期，找出人生中真正重要的事；PowerShell 的故事；好玩的个人主页

最近在一封邮件看到这段话：

> After a certain point, your goal is no longer to build a writing habit.
> 
> Your goal becomes falling so in love with interesting ideas that you *can’t not write about them*.
> 
> Curiosity breeds compulsion, and that’s far more important than forced consistency when trying to make work that’s fresh and inspired.

从读者角度来说，频繁更新的博客不一定值得频繁阅读，我们需要的是启发人的观点，而不是为了更新去写的内容，因为没有人能定时产生有价值的想法。

这段话来自 Julian Shapiro，就是我今天分享的第一篇文章的作者。

## 找出人生中真正重要的事

[How to figure out what to do with your life](https://www.julian.com/blog/life-planning)

Julian Shapiro 是一个软件开发者，创建过一个比较流行的 JavaScript 库 [julianshapiro/velocity](https://github.com/julianshapiro/velocity) ，也做过创业公司。

我订阅了他的 newsletter，他分享写作和个人成长方面的内容，文章都非常棒，你可以看看他的个人网站 [Julian Shapiro](https://www.julian.com/) 。

这篇文章中，他分享了如何确定不同人生阶段重大事项的优先级。我们需要定期去思考这些，因为随着年龄的增长，人的关注点和追求会改变。最近发现有的朋友也开始了第二人生，我想他们应该经过了类似的评估。

作者的方法包含以下几个维度：

![](https://catcoding.me/images/ob_2022-05-20-122353.png)

他基于这个方法评估出，自己不想再把做公司和挣钱放在第一位了，而写作优先级更高。但心里还有些犹豫，直到他看到 [Jeff Bezos 的一个访谈](https://www.youtube.com/watch?v=jwG_qR6XmDQ) 后有所顿悟。

Jeff Bezos 当时决定做亚马逊线上卖书的时候，使用了一个自称为 Regret Minimization Framework 的方法，简而言之就是： **假设当你 80 岁回首往事时，你会不会为不做这个事而遗憾？当你将未来的遗憾最小化时，你会睡得很香，因为你知道你在最大化地实现自己。**

这个词语有点技术化，不过和《钢铁是怎样炼成的》里的这句话是相同的：

> 人最宝贵的东西是生命。生命对人来说只有一次，因此，人的一生应当这样度过：当一个人回首往事时，不应虚度年华而悔恨，也不应碌碌无为而羞愧。

文章后面接着谈到钱的重要性和正确认知，这和我之前介绍过的 [最高形式的财富](https://catcoding.me/p/weekly-10/) 是一致的，钱能让人更自由，拒绝那些自己不想做的事。

人应该花更少的精力试图变得超级富有，而花更多的精力建立亲密关系、挚友圈，这些可以陪伴我们直到老去。

最后谈到 groupthink，每个人都属于自己所处的圈子，而这个圈子的人会对自己的认知造成很大的影响。为了打破趋同思维，我们需要不断问自己类似这样的问题：如果人生重来一次我想怎样？如果不缺钱我想做什么？

> I’ve noticed that many people compete in games they don’t understand because they are modeling the behavior of people around them. Most common is the competition for wealth as a proxy for happiness.
> 
> —Michael Seibel

从个人的经历来说，我似乎进入了低物欲的阶段，对电子产品都没兴趣了。最近花了很多时间看小说，把余华的主要作品看了一遍，我觉得这个年代的普通人都好幸福。

物欲的衰退也许是年龄和激素在作怪，谁知道呢，我觉得这样挺好。

## PowerShell 的故事

[Jeffrey Snover on Twitter](https://twitter.com/jsnover/status/1523010444570419200)

![](https://catcoding.me/images/ob_2022-05-20-143948.png)

Jeffrey Snover 是微软 Technical Fellow，这是不做管理的纯技术人员在微软的顶点，根据 [维基上的记录](https://en.wikipedia.org/wiki/Category:Microsoft_technical_fellows) ，目前一共只有 18 人。

Snover 在上面那个推特上回忆了自己最初做 PowerShell 原型而被降级的往事。这个故事也许你在其他新闻媒体上看到了，我们从技术角度来了解一下整个故事。

曾经，微软内部把开源和 Linux 视为敌人，对命令行这种风格的工具也是不屑一顾，甚至视为异己的：

> At the time, the “shell” project was viewed as a Linux-compete checkbox item of no importance whatsoever.

但 Snover 觉得自动化很重要，而 GUI 不适合做这方面，所以他做了这个 PowerShell 的原型，结果就是违反了公司主流而被降级。

Snover 坚持住了，他没有一味的把 Linux 那套 Shell 搬过来，而是借鉴了一些思想，然后根据 Windows 的环境和风格做了创新。光有理念和原型不够，也得有策略，在那些被压迫的日子里，他找到了公司内部的大用户 exchange，当真金白银投入到这个技术上之后，降级也不怕，没几年他就被晋升了。

他在这个 [访谈](https://evrone.com/jeffrey-snover-interview) 中回顾了更多当时的细节，Unix/Linux 的很多设计是基于文件和文本的，而 Windows 的设计是基于对象和 API 的，所以 PowerShell 管道中传递的是 Object 而不是文本，管道中也不像 Linux 那样都是跑的多个进程。

> Why invent PowerShell, why not just use ksh or bash? I’m a long time Unix dev so that was my first instinct. I tried and failed. There is a core architectural difference between Unix and Windows. Linux is a file-oriented OS and Windows is an API-oriented OS. In Linux, if you can modify a file and run a process, you can manage anything. That is why awk, sed, and grep are management tools. At the time, nothing on Windows worked that way. Everything was behind an API which returned a structured object.

后来 PowerShell 开始在微软自动化方面张露头角，并且随着新的 CEO Satya 宣布拥抱 Linux 和开源，以及微软整体上云的大趋势，PowerShell 成为不可缺少的基础设施和工具。

刚来微软的时候，我也觉得 PowerShell 好像挺奇怪的，熟悉了之后就觉得这东西很好！我们可以用命令行操作一个个对象，这些对象和.Net Object 是对应的，PowerShell 也可以和.Net 来交互，比如用 C# 来实现命令，而且现在也是开源跨平台了。

正在开发的 nushell 借鉴了 PowerShell 的这一理念 [nushell: A new type of shell](https://github.com/nushell/nushell)

## 好玩的个人主页

[Henry Heffernan - Portfolio 2022](https://henryheffernan.com/)

我非常羡慕那些既能编程又能做些设计的人，比如这位年轻的程序员，他的个人主页让人眼前一亮，强烈推荐你点进去看看：

![](https://catcoding.me/images/ob_2022-05-21-083853.png)

主页所有代码也是开源的： [henryjeff/portfolio-website](https://github.com/henryjeff/portfolio-website) ，使用了 TypeScript、three.js。类似的主页还有 [🚗 bruno-simon.com](https://bruno-simon.com/) ![](https://catcoding.me/images/ob_2022-05-21-084855.png)

即使是个人网站这样的小项目，这些人也能投入这么大精力和热情，玩出这么多花样。比如另一个前端工程师 Josh Comeau 这篇文章里分享了自己如何设计和实现个人网站 [How I Built my Blog using MDX, Next.js, and React](https://www.joshwcomeau.com/blog/how-i-built-my-blog/) ，其中那个动画人物的设计花了 500 美金。使用 MDX 可以构建出一些更具交互性的文章，这里面不仅有文字，还有对应的代码动画，比如 [Spring Physics animation in JavaScript](https://www.joshwcomeau.com/animation/a-friendly-introduction-to-spring-physics/) 。

这让我想起自己在知乎回答的 [为什么中国程序员不如外国程序员有创造性](https://www.zhihu.com/question/502884696/answer/2296787480) ，只有当我们有足够多的业余时间才能做出更多创造性的东西，这些创造性的东西可能不是为了名利，不是为了 KPI，只是为了好玩和分享，而那些伟大的项目 Linux、Ruby、Python 的源头都是 Just for fun。

再联想到 gitee 最近的代码审核，不禁心生悲哀。

## 其他

- 30 年软件开发学到了什么： [Julio Biason](https://blog.juliobiason.me/thoughts/things-i-learnt-the-hard-way/)
- 最近因为居家带娃上班，我需要带着笔记本去小区滑滑梯，所以使用触摸板时间多了，Thinkpad 的触摸板感觉比 Mac 差不少，但键盘体验很好。我就想着如何能提高效率，试着用了一下 Thinkpad 的小红帽，适应了一段时间感觉还不错，后来搜索发现了这个程序员的浏览器插件。如果你使用 VIM 和快捷键工具肯定会很喜欢这个 [philc/vimium: The hacker’s browser.](https://github.com/philc/vimium)

## 言论

![](https://catcoding.me/images/ob_2022-05-21-091310.png)

## Humor

![](https://catcoding.me/images/ob_2022-05-18-223422.png)

![](https://catcoding.me/images/wechat-qr-code.jpg)

公号同步更新，欢迎关注👻

<iframe title="Comments" src="https://utteranc.es/utterances.html?src=https%3A%2F%2Futteranc.es%2Fclient.js&amp;repo=chenyukang%2Fchenyukang.github.io&amp;issue-term=pathname&amp;theme=github-light&amp;crossorigin=anonymous&amp;async=&amp;url=https%3A%2F%2Fcatcoding.me%2Fp%2Fweekly-14%2F&amp;origin=https%3A%2F%2Fcatcoding.me&amp;pathname=p%2Fweekly-14%2F&amp;title=%E7%AC%AC+14+%E6%9C%9F%EF%BC%8C%E6%89%BE%E5%87%BA%E4%BA%BA%E7%94%9F%E4%B8%AD%E7%9C%9F%E6%AD%A3%E9%87%8D%E8%A6%81%E7%9A%84%E4%BA%8B%EF%BC%9BPowerShell+%E7%9A%84%E6%95%85%E4%BA%8B%EF%BC%9B%E5%A5%BD%E7%8E%A9%E7%9A%84%E4%B8%AA%E4%BA%BA%E4%B8%BB%E9%A1%B5+%7C+CatCoding&amp;description=All+about+coding+and+writing&amp;og%3Atitle=%E7%AC%AC+14+%E6%9C%9F%EF%BC%8C%E6%89%BE%E5%87%BA%E4%BA%BA%E7%94%9F%E4%B8%AD%E7%9C%9F%E6%AD%A3%E9%87%8D%E8%A6%81%E7%9A%84%E4%BA%8B%EF%BC%9BPowerShell+%E7%9A%84%E6%95%85%E4%BA%8B%EF%BC%9B%E5%A5%BD%E7%8E%A9%E7%9A%84%E4%B8%AA%E4%BA%BA%E4%B8%BB%E9%A1%B5+%7C+CatCoding&amp;session="></iframe>
