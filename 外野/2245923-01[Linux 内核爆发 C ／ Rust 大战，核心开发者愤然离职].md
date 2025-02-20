
*****

####  月灵银羽  
##### 1#       楼主       发表于 2025-2-11 20:05

 本帖最后由 月灵银羽 于 2025-2-12 11:02 编辑 

2月 11 日消息，Linux 内核社区近期爆发了一场关于编程语言的激烈争论，最终导致一位核心开发者退出项目。这场争论的核心在于是否应该更多地使用 Rust 语言来开发内核，以及开发者之间的沟通方式。

Asahi Linux 项目的领导者 Hector Martin 公开批评另一位资深内核开发者 Christoph Hellwig，阻碍 Rust 语言在内核中的应用。

Martin 认为，Rust 语言在内存管理方面更加安全和现代，应该在内核开发中扮演更重要的角色；而 Hellwig 则对从 C 语言迁移到 Rust 持谨慎态度，认为迁移过程会增加内核的复杂性，并直言在 Linux 中混用代码就是“癌症”。

Linux 之父 Linus Torvalds 的介入成为了事件的转折点。Torvalds 本人并不反对在内核中使用 Rust，但他对 Martin 公开批评 Hellwig 的方式表示强烈不满。

Torvalds 在内核邮件列表中批评 Martin，认为他应该反思自己的行为，并指出技术问题应该通过技术途径解决，而不是诉诸社交媒体。

在 Torvalds 的批评之后，Martin 宣布退出内核上游开发，转而专注于 Asahi Linux 的下游开发。他表示对内核开发流程和社区管理方式失去了信心，尽管如此，Martin 表示未来仍有可能向上游提交补丁。

[论坛助手,iPhone](https://bbs.saraba1st.com/2b/forum.php?mod=viewthread&amp;tid=2029836)

*****

####  i0ncube_R  
##### 2#       发表于 2025-2-11 20:15

看hackernews，kernel邮件列表上貌似吵了很久了

[论坛助手,iPhone](https://bbs.saraba1st.com/2b/forum.php?mod=viewthread&amp;tid=2029836)

*****

####  燕山雪  
##### 3#       发表于 2025-2-11 20:15

总觉得rust粉跟特么邪教一样

*****

####  双刀少女  
##### 4#       发表于 2025-2-11 20:15

一直想学rust，找不到应用场景啊...

*****

####  ryanz  
##### 5#       发表于 2025-2-11 20:20

这两者的矛盾本来就是不可调和的，最开始 rust 爱好者拿进内核来吹就觉得此事不长久。rust 需要 kernel 来证明自己，而 kernel 并不需要 rust 来保证所谓的安全性。

另外现在编译内核加个 ebpf 需要一堆依赖我就觉得麻烦的要死，更别提整另一个编译器依赖了。

*****

####  原装大小姐  
##### 6#       发表于 2025-2-11 20:22

rust确实蛮奇葩的，去到哪都想替换，从应用来看，替换造成的功能不可预期性比所谓的安全还值得担心

—— 来自 [鹅球](https://www.pgyer.com/xfPejhuq) v3.3.96-alpha

*****

####  weiyang  
##### 7#       发表于 2025-2-11 20:26

linus才55岁，就他这个级别来说不算老，起码还能镇压十年吧

*****

####  kumh  
##### 8#       发表于 2025-2-11 20:32

不如另开分支直接用rust实现完成kernel。

*****

####  thq  
##### 9#       发表于 2025-2-11 20:38

蟹粉为嘛不自己从头开始搞一个内核替代linux

*****

####  pwzzy  
##### 10#       发表于 2025-2-11 20:41

<img src="https://static.saraba1st.com/image/smiley/face2017/001.png" referrerpolicy="no-referrer">内核开发需要rust所谓的安全性吗，为了运行效率本来就允许用不安全的写法的，引入另一套体系复杂度不是爆炸了

*****

####  星空天神  
##### 11#       发表于 2025-2-11 20:55

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67397830&amp;ptid=2245923" target="_blank">pwzzy 发表于 2025-2-11 20:41</a>

内核开发需要rust所谓的安全性吗，为了运行效率本来就允许用不安全的写法的，引入另一套体系复杂度不是爆炸 ...</blockquote>
肯定一堆unsafe

*****

####  Nanachi  
##### 12#       发表于 2025-2-11 20:56

支持ruster重写kernel

—— 来自 [鹅球](https://www.pgyer.com/GcUxKd4w) v3.3.96

*****

####  厨具战士mk2  
##### 13#       发表于 2025-2-12 08:57

提到rust听到的大多都是重写，rust有没有自己的拳头应用？

*****

####  coyove  
##### 14#       发表于 2025-2-12 09:00

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67397779&amp;ptid=2245923" target="_blank"> kumh 发表于 2025-2-11 20:32</a> 不如另开分支直接用rust实现完成kernel。 </blockquote>
rinux，正好r l 不分来自: iPhone客户端

*****

####  幽箬筱  
##### 15#       发表于 2025-2-12 09:03

语言神批真的闹麻了

*****

####  YoumuChan  
##### 16#       发表于 2025-2-12 09:05

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67399873&amp;ptid=2245923" target="_blank">厨具战士mk2 发表于 2025-2-12 08:57</a>

提到rust听到的大多都是重写，rust有没有自己的拳头应用？</blockquote>
Cloudflare的Pingora算吗？

*****

####  Jet.Black  
##### 17#       发表于 2025-2-12 09:06

搞成这个样子，是不是Linus Torvalds本人受够了C语言，想用Rust?

*****

####  神圣天使书记官  
##### 18#       发表于 2025-2-12 09:07

没有拿得出手的东西只能靠吹是这样的

*****

####  iamawaistcoat  
##### 19#       发表于 2025-2-12 09:08

还不是linus放进来的

*****

####  montanaB  
##### 20#       发表于 2025-2-12 09:10

<blockquote>pwzzy 发表于 2025-2-11 20:41
内核开发需要rust所谓的安全性吗，为了运行效率本来就允许用不安全的写法的，引入另一套体系复杂度不是爆炸 ...</blockquote>
Rust这玩意儿最奇葩的是，搞了一大堆，各种概念，各种限制，来保证所谓的内存安全性。但是在这些东西之外，他居然也留了unsafe的后门。

我当时看到这一点后，我就对这语言的吹嘘失去了兴趣。如果他的安全性真的这么厉害，这么坚不可摧，那为什么要留后门？

*****

####  trentswd  
##### 21#       发表于 2025-2-12 09:13

上次俄罗斯贡献者那事咋样了，冷处理成功了？

*****

####  Midnight.Coup  
##### 22#       发表于 2025-2-12 09:13

用 rust 写的系统有啊，RedoxOS，用的 DE 也是 rust 写的 COSMIC Epoch 

*****

####  高妹控  
##### 23#       发表于 2025-2-12 09:20

印象里起码5、6年前，ruster就到处布道了，恨不得从今以后所有东西都要用rust写，到现在这个局面一点也不意外<img src="https://static.saraba1st.com/image/smiley/face2017/068.png" referrerpolicy="no-referrer">

—— 来自 [S1Fun](https://s1fun.koalcat.com)

*****

####  王兰花秀丽  
##### 24#       发表于 2025-2-12 09:20

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67399873&amp;ptid=2245923" target="_blank">厨具战士mk2 发表于 2025-2-12 08:57</a>

提到rust听到的大多都是重写，rust有没有自己的拳头应用？</blockquote>
区块链上面的solana，以及由基于rust的move语言的aptos和sui

*****

####  d2loader  
##### 25#       发表于 2025-2-12 09:34

<img src="https://static.saraba1st.com/image/smiley/face2017/112.png" referrerpolicy="no-referrer"> RIIR的人很多都很礼貌的

至少内核这件事上, C系开发者一个在别人演讲时突然打断演讲, 直球大喊大叫的

然后Christoph Hellwig说癌症

结果RIIR被泥潭骂邪教.... 

﹍﹍﹍

评分

 参与人数 1战斗力 +1

|昵称|战斗力|理由|
|----|---|---|
| darklinden| + 1|思维顽固了已经|

查看全部评分

*****

####  YoumuChan  
##### 26#       发表于 2025-2-12 09:36

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67399968&amp;ptid=2245923" target="_blank">montanaB 发表于 2025-2-12 09:10</a>

Rust这玩意儿最奇葩的是，搞了一大堆，各种概念，各种限制，来保证所谓的内存安全性。但是在这些东西之外 ...</blockquote>
因为通过Rice Theorem(莱斯定理)可以证明你不可能构造一个编译器使其接受所有内存安全的程序并拒绝所有内存不安全的程序。

Rust选择接受内存安全的程序的一个子集（从而把语义性质变为语法性质），通过unsafe让程序员在需要的时候自行写出内存安全集合与这个子集的差集。

﹍﹍﹍

评分

 参与人数 1战斗力 +1

|昵称|战斗力|理由|
|----|---|---|
| darklinden| + 1||

查看全部评分

*****

####  小止  
##### 27#       发表于 2025-2-12 09:37

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67399968&amp;ptid=2245923" target="_blank">montanaB 发表于 2025-2-12 09:10</a>

Rust这玩意儿最奇葩的是，搞了一大堆，各种概念，各种限制，来保证所谓的内存安全性。但是在这些东西之外 ...</blockquote>
按我理解用rust那套东西确实是可以实现所有功能，但是心智负担可能会增加到惊人的程度

*****

####  BetterCall  
##### 28#       发表于 2025-2-12 09:42

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67399888&amp;ptid=2245923" target="_blank">coyove 发表于 2025-2-12 09:00</a>
rinux，正好r l 不分</blockquote>
r l不分是什么意思？

—— 来自 [鹅球](https://www.pgyer.com/xfPejhuq) v3.3.96-alpha

*****

####  Steel.Haze  
##### 29#       发表于 2025-2-12 09:56

坚决抵制Rust作为内核。它针对内核开发，除了所谓的捕风捉影的"内存安全"之外，全无任何比较优势，缺点却很多，这个话题发展到目前的程度就是一种匪夷所思，而且针对未来的亲智能计算时代的计算架构来说更是灾难性的麻烦。这玩意现在被硬推有政治性，我甚至怀疑它最近这波被推动和某类美国情报部门特殊的网络攻击后门手段应用有关。

无论如何，如果有Rust混入内核，我肯定会用原来C系内核的搞自己的分支，不会接受。

﹍﹍﹍

评分

 参与人数 1战斗力 +1

|昵称|战斗力|理由|
|----|---|---|
| ForeverTime| + 1|+1|

查看全部评分

*****

####  darklinden  
##### 30#       发表于 2025-2-12 10:03

<img src="https://static.saraba1st.com/image/smiley/face2017/001.png" referrerpolicy="no-referrer">

“嘿兄弟，我知道你是十年经验的老走钢丝侠，但是你先别急，我给你推荐一辆走钢丝专用轮椅”

“这玩意儿纯钢打造，操作失误会挨鞭子，并且无法后退，无法跳跃，无法拿大顶”

“但是相信我，这玩意儿绝对可以保证小脑发育不全的人都能安全走钢丝，甚至有些情况下比你还快得多”

“并且像你这样的高手，也可以按下【unsafe】按钮跳出轮椅爱怎么跳怎么跳，当然以你的经验是不会摔的”

“你看以后你只需要在轮椅发展的过程中以你的高超能力做【unsafe】相关的工作，剩下的事情训练过的猴子都能干，是不是很棒啊？”

“你为什么要走？兄弟？什么？你为什么要砸了它？”

*****

####  小野賢章  
##### 31#       发表于 2025-2-12 10:04

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67399873&amp;ptid=2245923" target="_blank">厨具战士mk2 发表于 2025-2-12 08:57</a>

提到rust听到的大多都是重写，rust有没有自己的拳头应用？</blockquote>
从流行程度来看应该是 deno 和 Tauri，我自己用的最多的是 ripgrep，不过从功能来看这几个也都是广义重写，

排版软件 Typst 应该算原创<img src="https://static.saraba1st.com/image/smiley/face2017/067.png" referrerpolicy="no-referrer">

*****

####  カタカナジゴク  
##### 32#       发表于 2025-2-12 10:09

<img src="https://static.saraba1st.com/image/smiley/face2017/037.png" referrerpolicy="no-referrer">毕竟他们都写rust了<img src="https://p.sda1.dev/21/c16b2a8c35cbc2d3c36de9c24d01f4e9/image.jpg" referrerpolicy="no-referrer">

—— 来自 [鹅球](https://www.pgyer.com/xfPejhuq) v3.3.96-alpha

*****

####  迷路的石头  
##### 33#       发表于 2025-2-12 10:11

<blockquote>ryanz 发表于 2025-2-11 20:20
这两者的矛盾本来就是不可调和的，最开始 rust 爱好者拿进内核来吹就觉得此事不长久。rust 需要 kernel 来 ...</blockquote>
所以需要rust码农直接重写个runix

*****

####  montanaB  
##### 34#       发表于 2025-2-12 10:23

<blockquote>YoumuChan 发表于 2025-2-12 09:36
因为通过Rice Theorem(莱斯定理)可以证明你不可能构造一个编译器使其接受所有内存安全的程序并拒绝所有内 ...</blockquote>
既然从原理上就已经做不到了，那rust花费如此大的代价，就更不合算了。这套设计本来就对程序员的负担心智过重。我以前并不了解你说的这个原理，只是从直觉上觉得，无论是设计还是使用上，都付出了如此大的代价，却还是留下了不安全的后门，这不合理。现在你的说法更加坚定了我的想法：rust吹嘘的这套安全机制，并不能如他所说的那样，解决所有安全问题，他本质就跟Java语言的gc一样，是个为大部分场景设计的工具而已，但是Java的gc用起来很方便，你rust的安全系统，使用起来代价太大了

*****

####  montanaB  
##### 35#       发表于 2025-2-12 10:25

<blockquote>小止 发表于 2025-2-12 09:37
按我理解用rust那套东西确实是可以实现所有功能，但是心智负担可能会增加到惊人的程度 ...</blockquote>
如果真的能，那rust就不会为这套安全机制留个后门。楼上那位已经从理论上说明了，这套机制确实解决不了所有问题，只是一个子集，所以才留下unsafe的后门。

*****

####  r_ex  
##### 36#       发表于 2025-2-12 10:30

还是Rust自己写个内核吧。混合的东西确定不好

—— 来自 [鹅球](https://www.pgyer.com/GcUxKd4w) v3.3.96

*****

####  abcxiawei  
##### 37#       发表于 2025-2-12 10:34

 本帖最后由 abcxiawei 于 2025-2-12 10:39 编辑 
<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67400314&amp;ptid=2245923" target="_blank">Steel.Haze 发表于 2025-2-12 09:56</a>

坚决抵制Rust作为内核。它针对内核开发，除了所谓的捕风捉影的"内存安全"之外，全无任何比较优势，缺点却很 ...</blockquote>
如果rust真的能彻底解决内存安全问题，我不介意它代替其它语言，毕竟内存安全是个非常麻烦的问题。

问题恰恰是rust解决不了内存安全问题。我以前仅仅是直觉上觉得如此——你rust真能解决内存安全问题为什么要留unsafe后门呢？

现在好了，楼上有个理论大拿直接从定理证明，能彻底解决内存安全的编译器至少目前不存在！

那你rust花了那么大代价——无论是设计还是使用上——程序员用起你这个安全系统痛苦万分，付出如此大的代价后，发现你这东西其实是个半拉子，根本构建不起吹嘘的【彻底解决内存安全问题】的宏大叙事，那意义何在？

解决内存安全的半拉子工程现在就有样板：各个带有内存回收的语言，人家也是半拉子，解决不了所有内存安全问题，问题是人家这个半拉子给程序员用起来没有心智负担啊。

rust没戏，我以前只是直觉觉得如此，看了26楼那位大佬从基础理论论述为啥rust必须留unsafe后门后，我现在反而更坚定了这点。

*****

####  Steel.Haze  
##### 38#       发表于 2025-2-12 10:49

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67400650&amp;ptid=2245923" target="_blank">abcxiawei 发表于 2025-2-12 10:34</a>

如果rust真的能彻底解决内存安全问题，我不介意它代替其它语言，毕竟内存安全是个非常麻烦的问题。</blockquote>
是的，我也觉得肯定解决不了，内存安全怎么能单靠换个语言写法就搞定。不光是unsafe问题。编写的逻辑错误、FFI 交互等等都是不可避免的。

而且原则上，我觉得编译越麻烦的语言框架解决起来越难。所以现在的Linux的内核已经是一种接近逻辑、应用需求和简洁度相对自洽的状态。一旦混入Rust，那么可能造成的污染和带来的问题非常不可测。现在内核核心子系统（如调度、内存管理）高度依赖C语言实现的复杂数据结构与宏，Rust的强类型系统和所有权模型难以直接兼容，需通过大量 unsafe代码桥接，削弱安全性优势，甚至直接操作MMIO寄存器也要unsafe实现。本质上，引入混用，将直接给Linux内核在内存安全上开口子，而不是增强。而Linux内核层突破其实一直是美国情报机构想要“更便利”解决的一个问题。

而且本质上，目前unsafe代码需人工验证其正确性，但内核规模的代码库中，此类代码的交互可能引入难以追踪的底层问题。引入Rust后，实际上这部分安全性就拿捏到代码提交者手上，本质上这个也是一种“夺权”。

*****

####  a317216007  
##### 39#       发表于 2025-2-12 10:59

<img src="https://static.saraba1st.com/image/smiley/face2017/048.png" referrerpolicy="no-referrer">所以如果rust真的那么牛逼，为什么不直接重构一个内核分支去证明自己牛逼，而是老想着鹊巢鸠占

说白了这件事就根本不是技术驱动而是利益驱动罢了

*****

####  d2loader  
##### 40#       发表于 2025-2-12 11:00

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67400650&amp;ptid=2245923" target="_blank">abcxiawei 发表于 2025-2-12 10:34</a>
如果rust真的能彻底解决内存安全问题，我不介意它代替其它语言，毕竟内存安全是个非常麻烦的问题。</blockquote>
只是对你个人而已觉得心智负担大吧

但是新成长起来的00后码农很多人都会

—— 来自 [鹅球](https://www.pgyer.com/GcUxKd4w) v3.3.96


*****

####  d2loader  
##### 41#       发表于 2025-2-12 11:01

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67400901&amp;ptid=2245923" target="_blank">a317216007 发表于 2025-2-12 10:59</a>
所以如果rust真的那么牛逼，为什么不直接重构一个内核分支去证明自己牛逼，而是老想着鹊巢鸠占

说白了这件 ...</blockquote>
redoxOS项目并没有停止开发

—— 来自 [鹅球](https://www.pgyer.com/GcUxKd4w) v3.3.96

*****

####  takitaki  
##### 42#       发表于 2025-2-12 11:02

不知道为什么，rust爱好者越赞美rust，我越觉得这玩意后门多的数不胜数<img src="https://static.saraba1st.com/image/smiley/face2017/009.gif" referrerpolicy="no-referrer">


*****

####  manysun  
##### 43#       发表于 2025-2-12 11:08

rust崩溃论：unsafe
rust威 胁论：进Linux内核

然后每天用RIIR的东西。

*****

####  YoumuChan  
##### 44#       发表于 2025-2-12 11:14

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67400650&amp;ptid=2245923" target="_blank">abcxiawei 发表于 2025-2-12 10:34</a>

如果rust真的能彻底解决内存安全问题，我不介意它代替其它语言，毕竟内存安全是个非常麻烦的问题。</blockquote>
我觉得”如果一门语言无法完全解决内存安全问题，则无意义“是一个比较极端的想法。

对于C/C++来说，可以认为全部文件所有地方都是unsafe，所以内存安全问题可以出现在任意文件的任意地方。

rust的理念是，如果所有unsafe的地方都是sound的，那么编译器可以证明所有没有unsafe的地方一定也都是sound的。tradeoff是没有unsafe的地方会有一些比较严格的生命周期限制。

其实这种渐进的改进是有益的，毕竟缩小了攻击介面，一是绝大部分的business logic都不会有unsafe，unsafe一般占比是很小的。二是unsafe是一个显式的标志，很容易grep出来。那么做audit的时候可以集中考虑unsafe的部分，debug的时候也可以比较容易定位unsafe。

我写了快10年C/C++后来接触rust，我觉得rust把一些写C/C++脑子里需要自己维护的东西（生命周期）显性地表示出来其实反而降低了一些心智负担。据我观察，在C/C++中踩过的坑越多，对于rust上手越快。


*****

####  abcxiawei  
##### 45#       发表于 2025-2-12 11:16

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67400911&amp;ptid=2245923" target="_blank">d2loader 发表于 2025-2-12 11:00</a>

只是对你个人而已觉得心智负担大吧

但是新成长起来的00后码农很多人都会</blockquote>
又是这套“我头脑比你强”逻辑。

我自己也是程序员出身的。我已经不止一次看到你们这种逻辑了，越年轻的程序员往往越有这种自信。

可是朋友，心智负担这个东西，不是看人聪明不聪明，是看你用的编程工具方便不方便来比较的。

在一大票解决内存安全半拉子语言自带的内存回收面前，你rust那花里胡哨的设计，就是心智负担过重，作为工具，内存回收用起来难道不比rust那套所有权机制简单方便？

当汽车全部标配方向盘液压助力的时候，你开个没有方向盘助力的车，并向开有助力的司机表示：是你自己觉得方向盘重不好转吧，新成长起来的年轻人转的很好啊。。。

编程这个东西，从发展到现在，越来越偏向一个工具，工具就是要越简单，越多人能用为好，如果一个工具发明出来，解决问题的效果和其他工具区别不大，反而用起来难了很多，那它对使用者就是负担。这个不以使用者自身能力如何而决定。

上世纪80年代的时候，学术界曾经争论过HaskWell和C语言，谁会是新时代的主宰，那会几乎所有的专业人士，都更看好HaskWell，当时有个说法，说“HaskWell是给聪明人的设计，而C语言简陋，是为愚笨的人的设计”。最后如何呢，更“简陋”的C语言征服了世界，因为普通人用C语言比用HaskWell要容易的多


*****

####  abcxiawei  
##### 46#       发表于 2025-2-12 11:27

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67401032&amp;ptid=2245923" target="_blank">YoumuChan 发表于 2025-2-12 11:14</a>

我觉得”如果一门语言无法完全解决内存安全问题，则无意义“是一个比较极端的想法。

对于C/C++来说，可以 ...</blockquote><blockquote>如果一门语言无法完全解决内存安全问题，则无意义</blockquote>不，你曲解了我的话，我不是认为没意义。而是，你不能付出如此巨大的代价后，最后实现的效果和别人家更简单的方式差不多。

rust这套机制，它实际不是解决问题，它是把新问题暴露在编译前，你作为一个已经写了10多年C、C++的人，对C系内存管理的弱点非常熟悉，所以你用rust，会有一种太好了，这玩意把问题在编译前暴露给我了，你肯定会觉得找到知己了。

但是对于没有这方面经验的人来说，第一步就被拦住了。

rust并没有解决问题，它只是把入门门槛抬起来，直接不让没有经验的人进来而已。

这看起来很美好，但是其实它把自己的路给堵了。我前面说，HaskWell和C语言的历史争论，最后是“更简陋，更为愚笨的人设计”的C语言赢了的


*****

####  abcxiawei  
##### 46#       发表于 2025-2-12 11:27

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67401032&amp;ptid=2245923" target="_blank">YoumuChan 发表于 2025-2-12 11:14</a>

我觉得”如果一门语言无法完全解决内存安全问题，则无意义“是一个比较极端的想法。

对于C/C++来说，可以 ...</blockquote><blockquote>如果一门语言无法完全解决内存安全问题，则无意义</blockquote>不，你曲解了我的话，我不是认为没意义。而是，你不能付出如此巨大的代价后，最后实现的效果和别人家更简单的方式差不多。

rust这套机制，它实际不是解决问题，它是把新问题暴露在编译前，你作为一个已经写了10多年C、C++的人，对C系内存管理的弱点非常熟悉，所以你用rust，会有一种太好了，这玩意把问题在编译前暴露给我了，你肯定会觉得找到知己了。

但是对于没有这方面经验的人来说，第一步就被拦住了。

rust并没有解决问题，它只是把入门门槛抬起来，直接不让没有经验的人进来而已。

这看起来很美好，但是其实它把自己的路给堵了。我前面说，HaskWell和C语言的历史争论，最后是“更简陋，更为愚笨的人设计”的C语言赢了的


*****

####  云卷花开  
##### 47#       发表于 2025-2-12 11:38

编辑。。。


*****

####  darklinden  
##### 48#       发表于 2025-2-12 11:51

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67401158&amp;ptid=2245923" target="_blank">abcxiawei 发表于 2025-2-12 11:27</a>

不，你曲解了我的话，我不是认为没意义。而是，你不能付出如此巨大的代价后，最后实现的效果和别人家更简 ...</blockquote>
恰恰相反，你看到的“高门槛”在目前ai助手满地的情况下根本不是事儿

ai满嘴胡话的情况下，rust编译器的小皮鞭抽着更容易写出健壮代码，而gc语言闹oom的几率则是**（糊哩哗啦）增加的

00后随便拉个无经验和ai聊天用rust做小脚本儿还能调优根本不是事儿，反而写着测试着没事儿跑一两天崩了才是头疼玩意儿

时代变了，老哥
<img src="https://static.saraba1st.com/image/smiley/face2017/002.png" referrerpolicy="no-referrer">


*****

####  abcxiawei  
##### 49#       发表于 2025-2-12 12:03

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67401345&amp;ptid=2245923" target="_blank">darklinden 发表于 2025-2-12 11:51</a>

恰恰相反，你看到的“高门槛”在目前ai助手满地的情况下根本不是事儿

ai满嘴胡话的情况下，rust编译器的小 ...</blockquote>
那我们就继续看，看rust到底能不能在这个领域把C和C++的地盘侵蚀掉好了。

AI可以教人写rust脚本，照样可以教C和C++脚本，而且，越没门槛，AI教的越好，这是我的判断

*****

####  ryanz  
##### 50#       发表于 2025-2-12 12:07

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67401345&amp;ptid=2245923" target="_blank">darklinden 发表于 2025-2-12 11:51</a>

恰恰相反，你看到的“高门槛”在目前ai助手满地的情况下根本不是事儿

ai满嘴胡话的情况下，rust编译器的小 ...</blockquote>
这种涉及借用权的恰恰 ai 可能绕不过那么多弯。昨天遇见群里有人问一个问题就顺道去问了 ai 

can the code run

fn main() {

    let mut v = vec![1, 3, 4, 5]; 

    v[v.len() - 1] = 4; 

    println!("{:?}", v); 

} 

ai 答错了，而正确的解答在这里 [https://users.rust-lang.org/t/ca ... ed-as-mutable/85785](https://users.rust-lang.org/t/cannot-borrow-as-immutable-because-it-is-also-borrowed-as-mutable/85785) 作为老早就在我书签里 2022 年的问答它应该学习到才对。


*****

####  redbuck  
##### 51#       发表于 2025-2-12 12:15

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67399968&amp;ptid=2245923" target="_blank">montanaB 发表于 2025-2-12 09:10</a>
Rust这玩意儿最奇葩的是，搞了一大堆，各种概念，各种限制，来保证所谓的内存安全性。但是在这些东西之外 ...</blockquote>
逃生窗肯定要留的，这不算啥黑点

*****

####  Vacuolar  
##### 52#       发表于 2025-2-12 12:17

这个吵了得有两年了吧


*****

####  IIIIIlllllIIIII  
##### 53#       发表于 2025-2-12 12:20

<img src="https://static.saraba1st.com/image/smiley/face2017/018.png" referrerpolicy="no-referrer">
经典笑话之评论c和rust 哪个好
答案是高级c++
“我不知道 因为我用concepts和constexpr”

— from [S1 Next Goose](https://www.pgyer.com/GcUxKd4w) v3.3.96


*****

####  d2loader  
##### 54#       发表于 2025-2-12 12:41

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67401158&amp;ptid=2245923" target="_blank">abcxiawei 发表于 2025-2-12 11:27</a>

不，你曲解了我的话，我不是认为没意义。而是，你不能付出如此巨大的代价后，最后实现的效果和别人家更简 ...</blockquote>
大哥, 你用C/C++上班工作一样要开各种静态检查和santinizer的, 还有调试必须会valgrind和gdb这些

你都会这么多东西了看看rust上手很容易的, 使用也不复杂

*****

####  白日依山尽  
##### 55#       发表于 2025-2-12 12:42

rust是面向老板编程，各类问题都要考虑到处理好，不然都跑不起来，一旦跑起来后续出现的问题几率相对小，不增减功能完全可以把程序员开了。

C之类就相反，把主要逻辑走通，跑起来再说，后面有问题再慢慢修，或许很久才出现当时没预计到的问题，不过这个时候可能程序员都已经换几个公司了。


*****

####  darklinden  
##### 56#       发表于 2025-2-12 12:45

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67401446&amp;ptid=2245923" target="_blank">ryanz 发表于 2025-2-12 12:07</a>

这种涉及借用权的恰恰 ai 可能绕不过那么多弯。昨天遇见群里有人问一个问题就顺道去问了 ai 

can the cod ...</blockquote>

对于应用来说...ai应该...还行？

<img src="https://img.saraba1st.com/forum/202502/12/124352ie6jbi2ee63vje9x.png" referrerpolicy="no-referrer">

<strong>wtf.png</strong> (39.88 KB, 下载次数: 0)

下载附件

2025-2-12 12:43 上传


*****

####  ryanz  
##### 57#       发表于 2025-2-12 12:57

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67401733&amp;ptid=2245923" target="_blank">darklinden 发表于 2025-2-12 12:45</a>

对于应用来说...ai应该...还行？</blockquote>
公司禁止用 copilot 不太了解关于它修复代码的原理，猜测可能因为编辑器的 linter 告诉 copilot 它才知道错了，这个猜测不一定对。直接拿这段代码问过 deepseek 和 chatgpt，它们都认为可以得到结果。

*****

####  YoumuChan  
##### 58#       发表于 2025-2-12 12:57

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67401158&amp;ptid=2245923" target="_blank">abcxiawei 发表于 2025-2-12 11:27</a>

不，你曲解了我的话，我不是认为没意义。而是，你不能付出如此巨大的代价后，最后实现的效果和别人家更简 ...</blockquote>
那么你可以说rust有很陡峭的学习曲线，但我觉得跟加强心智负担是有区别的。

而C/C++也只不过是把rust陡峭的部分，藏在一次次的segmentation fault，gdb和asan中而已。

我个人其实觉得语言学习的第一门语言不应该是rust，先C/C++起手，延迟一小段时间再开始rust其实对于语言之间的tradeoff会有更好的理解。而跟rust编译器搏斗学到的生命周期，反过来对于写C/C++也是有帮助的，可以对于写C/C++潜移默化学到的内存安全规则形成更系统的理解。


*****

####  bcxzzz  
##### 59#       发表于 2025-2-12 13:03

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67399968&amp;ptid=2245923" target="_blank">montanaB 发表于 2025-2-12 09:10</a>
Rust这玩意儿最奇葩的是，搞了一大堆，各种概念，各种限制，来保证所谓的内存安全性。但是在这些东西之外 ...</blockquote>
对于这种后出来的语言，美国的棱镜计划之类的，会不会直接在编译器里埋后门？

—— 来自 HUAWEI LIO-AL00, Android 12上的 [S1Next-鹅版](https://github.com/ykrank/S1-Next/releases) v2.5.4


*****

####  Jet.Black  
##### 60#       发表于 2025-2-12 13:08

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67401866&amp;ptid=2245923" target="_blank">bcxzzz 发表于 2025-2-12 13:03</a>

对于这种后出来的语言，美国的棱镜计划之类的，会不会直接在编译器里埋后门？

—— 来自 HUAWEI LIO-AL0 ...</blockquote>
肯定有啊，美国政府强推Rust，你以为他们真关心技术啊。

<img src="https://static.saraba1st.com/image/smiley/face2017/043.png" referrerpolicy="no-referrer">


*****

####  d2loader  
##### 61#       发表于 2025-2-12 13:15

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67401893&amp;ptid=2245923" target="_blank">Jet.Black 发表于 2025-2-12 13:08</a>

肯定有啊，美国政府强推Rust，你以为他们真关心技术啊。</blockquote>
你们到底在胡说什么啊.... 华为是唯一非美国的rust基金会白金赞助商

而且servo项目被华为接过来了准备以后做鸿蒙webview的底层, 做自己掌控的浏览器

<img src="https://static.saraba1st.com/image/smiley/face2017/003.png" referrerpolicy="no-referrer">


*****

####  Jet.Black  
##### 62#       发表于 2025-2-12 13:26

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67401936&amp;ptid=2245923" target="_blank">d2loader 发表于 2025-2-12 13:15</a>

你们到底在胡说什么啊.... 华为是唯一非美国的rust基金会白金赞助商

而且servo项目被华为接过来了准备以 ...</blockquote>
想表达啥？华为又不是神，傻逼事情可没少干。

美国政府几次三番强推Rust不是新闻了，没有其他目的我是不信的。


*****

####  白笛之音  
##### 63#       发表于 2025-2-12 13:30

作为modern c++的用户，我能理解rust要干什么，但我觉得他们的解决方式不甚雅观（当然c++可能有不雅观的部分和历史包袱）

深入到实际的软件工程，rust带来的不甚可靠的安全性就未必值得给linux这样的成熟项目额外带来工程上的复杂度了。


*****

####  montanaB  
##### 64#       发表于 2025-2-12 13:37

<blockquote>redbuck 发表于 2025-2-12 12:15
逃生窗肯定要留的，这不算啥黑点</blockquote>
rust如果不吹它那一套“”彻底解决内存安全问题“”那这就不是黑点。问题是rust天天在吹这个，那这个逃生窗就成了个笑话

*****

####  montanaB  
##### 65#       发表于 2025-2-12 13:37

<blockquote>bcxzzz 发表于 2025-2-12 13:03
对于这种后出来的语言，美国的棱镜计划之类的，会不会直接在编译器里埋后门？

—— 来自 HUAWEI LIO-AL0 ...</blockquote>
你谈的是另外一个层面的问题


*****

####  abcxiawei  
##### 66#       发表于 2025-2-12 13:43

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67401825&amp;ptid=2245923" target="_blank">YoumuChan 发表于 2025-2-12 12:57</a>

那么你可以说rust有很陡峭的学习曲线，但我觉得跟加强心智负担是有区别的。

而C/C++也只不过是把rust陡峭 ...</blockquote>
没心智负担怎么会那么多和编译器搏斗的笑话？你别和我说这都是程序员水平不行造成的，当一个工具开始使劲强调使用者的水平的时候，它的竞争力就要下降了。

不好用就是不好用，不用给工具找理由。

要解决内存安全性问题的初衷没有错，但是rust的这个解法肯定是有问题的，学习曲线陡，使用起来照样困难。

我没有说C/C++容易，实际上这两个语言也是以难度高，难以精通著称的。

而且：rust搞了大堆眼花缭乱的东西，难度没降低，最终也没解决内存安全问题。然后声称要取代C/C++。。。

rust只是用一个问题掩盖另外一个问题，这个搞法从方法论上来说就不对。

*****

####  ywydsd  
##### 67#       发表于 2025-2-12 13:43

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67399968&amp;ptid=2245923" target="_blank">montanaB 发表于 2025-2-12 09:10</a>
Rust这玩意儿最奇葩的是，搞了一大堆，各种概念，各种限制，来保证所谓的内存安全性。但是在这些东西之外 ...</blockquote>
可能就是为了留后门

—— 来自 [鹅球](https://www.pgyer.com/xfPejhuq) v3.3.96-alpha

*****

####  万恶淫猥手  
##### 68#       发表于 2025-2-12 13:45

Rust 粉和 NodeJS 粉已经快接近之前的 PHP 了<img src="https://static.saraba1st.com/image/smiley/face2017/053.png" referrerpolicy="no-referrer">


*****

####  abcxiawei  
##### 69#       发表于 2025-2-12 13:49

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67401711&amp;ptid=2245923" target="_blank">d2loader 发表于 2025-2-12 12:41</a>

大哥, 你用C/C++上班工作一样要开各种静态检查和santinizer的, 还有调试必须会valgrind和gdb这些

你都会 ...</blockquote>
我没觉得C/C++简单，本来这就是两个难以学习和精通的语言。

所以我也不觉得rust容易。

问题是rust搞了这么多东西后，内存安全问题没有解决啊。

用rust的和编译器搏斗的困难，取代和C/C++的各种漏内存，异常等搏斗的困难，最后，内存安全问题还是没有解决。

为啥要换呢？找不到足够的理由啊。

你愿意换是你的自由。但我觉得当一个语言没有解决既往语言面对的问题的时候，那它的存在价值就是要打问号的。


*****

####  darklinden  
##### 70#       发表于 2025-2-12 14:15

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67401819&amp;ptid=2245923" target="_blank">ryanz 发表于 2025-2-12 12:57</a>

公司禁止用 copilot 不太了解关于它修复代码的原理，猜测可能因为编辑器的 linter 告诉 copilot 它才知道 ...</blockquote>

claude, copilot一开始死不悔改说没错，但是认编译器报错，可以正确提示修改意见

ds问了死不悔改说没错，再问busy了就没试成编译器错误信息回复，理论上应该会认...

gpt不开search和reason也是死不悔改，开了就一次过...

<img src="https://img.saraba1st.com/forum/202502/12/140937qchs38dchmnac8f7.png" referrerpolicy="no-referrer">

<strong>wtf.png</strong> (280.66 KB, 下载次数: 0)

下载附件

2025-2-12 14:09 上传

﹍﹍﹍

评分

 参与人数 1战斗力 +2

|昵称|战斗力|理由|
|----|---|---|
| ryanz| + 2|欢乐多|

查看全部评分


*****

####  pigbayspy  
##### 71#       发表于 2025-2-12 14:46

写过 c++ 的人就知道 rust 有多好了

真的是彻底地把 c++ 底下哪些要自己注意的一堆隐式的东西都给你暴露出来了

虽然暴露出来的这些限制，会让完成一些东西很困难（著名的rust新手第一步写个双向链表

但是真的从工程实践上来说，规避了很多坑


*****

####  phorcys02  
##### 72#       发表于 2025-2-12 15:02

rust的问题和node一样，是 crates.io


*****

####  woodey  
##### 73#       发表于 2025-2-12 15:58

 本帖最后由 woodey 于 2025-2-12 15:59 编辑 

我知道rust很好，那为啥不用rust新做一个系统？<img src="https://static.saraba1st.com/image/smiley/face2017/001.png" referrerpolicy="no-referrer">


*****

####  Steel.Haze  
##### 74#       发表于 2025-2-12 16:27

 本帖最后由 Steel.Haze 于 2025-2-12 16:29 编辑 
<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67401032&amp;ptid=2245923" target="_blank">YoumuChan 发表于 2025-2-12 11:14</a>

我觉得”如果一门语言无法完全解决内存安全问题，则无意义“是一个比较极端的想法。

对于C/C++来说，可以 ...</blockquote>
你这个说法太理中客。且不说换内核的整体工程代价。这种集中化模式其实增加易于被几种攻击的点而已。你只是初摸rust觉得好上手问题。这个主题讨论的是用rust去换linux的内核和混入内核，不是写个小应用。这个前提问题就不一样。rust这个架构必然是只是一种“过客”语言，一种语言有个局部优势就去奉若神明，甚至拿去替换核心OS的内核，然后这个漫长的工程推进中，它本身就已经过时了，变成了一种不上不下漏洞明显的产物。这样的语言我们见得还少吗？rust又不是最近才出来的吧？它真有竞争力早该被主动在内核领域开始应用了。不需要这么激烈的碰撞来推动。反而rust在话题热度了一段时间后被很多人抛弃了，是最近又被翻出来炒作吧，为了配合混入linux内核和替代部分其它内核与底层程序在炒作吧？而且有美国政府参与推动吧？为什么呢？


*****

####  yvev  
##### 75#       发表于 2025-2-12 17:20

这怎么从rust不能进内核歪到rust是天下第一cjb语言了。反正rust再怎么烂也还是“现代语言”，至于能不能进内核，反正c++进不去<img src="https://static.saraba1st.com/image/smiley/face2017/067.png" referrerpolicy="no-referrer">


*****

####  d2loader  
##### 76#       发表于 2025-2-12 17:42

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67403526&amp;ptid=2245923" target="_blank">Steel.Haze 发表于 2025-2-12 16:27</a>
你这个说法太理中客。且不说换内核的整体工程代价。这种集中化模式其实增加易于被几种攻击的点而已。你只 ...</blockquote>
<img src="https://static.saraba1st.com/image/smiley/face2017/003.png" referrerpolicy="no-referrer">
根本不是你说的能阻止或者禁止的，现在是个人按照教程就能用rust写内核驱动

—— 来自 [鹅球](https://www.pgyer.com/GcUxKd4w) v3.3.96


*****

####  samfs  
##### 77#       发表于 2025-2-12 17:47

非计算机专业，图一乐的话，rust 值得学吗，和 C 比呢

*****

####  ryanz  
##### 78#       发表于 2025-2-12 17:50

<blockquote>samfs 发表于 2025-2-12 17:47
非计算机专业，图一乐的话，rust 值得学吗，和 C 比呢</blockquote>
图一乐现在学 python 玩最火的 ai 吧。


*****

####  yxz_00  
##### 79#       发表于 2025-2-12 17:55

Rust是一门很值得学的语言. 写了几千行rust之后再回去写C++我感觉到了自己的功力提升 (我有10年C++经验)

然而Rust过于复杂了, 说简单的人我打赌它们没有认真设计过一个跨线程的rust框架, 或者就是很多流氓ruster说的那种, "搞不懂生命周期? 拷贝就行."

另外, rust的宏对我来说比C的宏还难以阅读.

这么复杂的一个语言生产力是存疑的, 他能吸引的智力也是存疑的. 我想这也是为什么至今rust还没有自己拿的出手的大应用. 而是热衷于跑去重写别人的系统来证明自己. 

同时既要面对现实需求的复杂度, 又要面对语言本身的复杂度, 再牛逼的人都会心累. 重写至少只用面对后者.

至于说什么AI帮忙, AI如果写rust牛逼, 写C++只会更牛逼.


*****

####  bcxzzz  
##### 80#       发表于 2025-2-12 18:02

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67402093&amp;ptid=2245923" target="_blank">montanaB 发表于 2025-2-12 13:37</a>

你谈的是另外一个层面的问题</blockquote>
从技术上来说，可能给一种语言留后门么？ 比如考虑下：1、语言的解释器、编译器是公开代码的么？ 2，即使在语言中留了某个后门，怎么让它在预定的地方起作用？  从技术上说，这能实现不？


*****

####  我是蓝石头  
##### 81#       发表于 2025-2-12 18:10

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67404180&amp;ptid=2245923" target="_blank">samfs 发表于 2025-2-12 17:47</a>
非计算机专业，图一乐的话，rust 值得学吗，和 C 比呢</blockquote>
建议python，一个上午就可以零到一写一个简单的有监督机器学习训练加推理，感受朴素的机器学习乐趣。
再花一个下午可以零到一部署一个带前端，带后端，带数据库，甚至还有api看板的全栈应用。
再花一个上午，把自带的文件上传接口后面接上刚训练的那个模型的推理，好了，你有了一个图片分类站点<img src="https://static.saraba1st.com/image/smiley/face2017/172.png" referrerpolicy="no-referrer">


*****

####  非教徒  
##### 82#       发表于 2025-2-12 18:57

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67404353&amp;ptid=2245923" target="_blank">我是蓝石头 发表于 2025-2-12 18:10</a>

建议python，一个上午就可以用pytorch零到一写一个简单的有监督机器学习训练加推理，感受朴素的机器学习 ...</blockquote>
来个教程的链接啊...


*****

####  iamawaistcoat  
##### 83#       发表于 2025-2-12 18:58

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67404297&amp;ptid=2245923" target="_blank">bcxzzz 发表于 2025-2-12 18:02</a>

从技术上来说，可能给一种语言留后门么？ 比如考虑下：1、语言的解释器、编译器是公开代码的么？ 2，即使 ...</blockquote>
和npm一样，在cargo拉进来的那一堆依赖里面？

*****

####  Xerxes_2  
##### 84#       发表于 2025-2-12 19:03

看这个帖子就高潮的人是不是根本对前情没有一点了解就来输出的？

首先 Rust 进 Linux 是 Linus 本人首肯的，C++都没进

其次前几个月在 Rust4Linux 会议上有 C 的支持者当众指着鼻子骂，这才是这些纷争的导火索


*****

####  samfs  
##### 85#       发表于 2025-2-12 19:59

<blockquote>ryanz 发表于 2025-2-12 17:50
图一乐现在学 python 玩最火的 ai 吧。</blockquote>
有一说一确实可以试试

*****

####  samfs  
##### 86#       发表于 2025-2-12 19:59

<blockquote>我是蓝石头 发表于 2025-2-12 18:10
建议python，一个上午就可以用pytorch零到一写一个简单的有监督机器学习训练加推理，感受朴素的机器学习 ...</blockquote>
看描述确实很有乐趣


*****

####  Steel.Haze  
##### 87#       发表于 2025-2-12 20:02

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67404132&amp;ptid=2245923" target="_blank">d2loader 发表于 2025-2-12 17:42</a>

根本不是你说的能阻止或者禁止的，现在是个人按照教程就能用rust写内核驱动</blockquote>
实际上我说这些的主要感觉就是rust进内核就是有推手搞起来的一阵风，各个社区都有抵制情绪，再结合上面的提到的情况，最终无疾而终。能写当然是肯定能写。不过其最终不会占据一偶。

*****

####  abcxiawei  
##### 88#       发表于 2025-2-12 20:03

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67404180&amp;ptid=2245923" target="_blank">samfs 发表于 2025-2-12 17:47</a>

非计算机专业，图一乐的话，rust 值得学吗，和 C 比呢</blockquote>
不值，非计算机专业请一切围绕你要实现的东西走，哪个语言能最快的实现出你想要的东西，你就用哪个，没必要一定用rust，甚至没必要一定用C


*****

####  abcxiawei  
##### 89#       发表于 2025-2-12 20:05

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67404685&amp;ptid=2245923" target="_blank">非教徒 发表于 2025-2-12 18:57</a>

来个教程的链接啊...</blockquote>
教程？随便打开个AI，问它：

1.我想要个什么，应该用什么实现

巴拉巴拉巴拉巴拉巴拉巴拉巴拉巴拉巴拉巴拉

2.这个东西需要什么样的环境，怎么搭

巴拉巴拉巴拉巴拉巴拉巴拉巴拉巴拉巴拉巴拉

3.环境搭好了，请给我写一个范例程序

巴拉巴拉巴拉巴拉巴拉巴拉巴拉巴拉巴拉巴拉

*****

####  Wiksy  
##### 90#       发表于 2025-2-12 20:06

<blockquote>samfs 发表于 2025-2-12 17:47
非计算机专业，图一乐的话，rust 值得学吗，和 C 比呢</blockquote>
非专业的就用各种脚本语言平时做工具就挺好的了，不需要C或者rust这种


*****

####  darklinden  
##### 91#       发表于 2025-2-12 20:19

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67404748&amp;ptid=2245923" target="_blank">Xerxes_2 发表于 2025-2-12 19:03</a>
看这个帖子就高潮的人是不是根本对前情没有一点了解就来输出的？

首先 Rust 进 Linux 是 Linus 本人首肯的 ...</blockquote>
他们只是想骂 rust 而已 <img src="https://static.saraba1st.com/image/smiley/face2017/002.png" referrerpolicy="no-referrer">

这事儿吧…
Linus 允许 rust 进 驱动

某个讲座上说的是“只是想了解或者精细化每个变量的生命周期以使其更加安全”然后被嘘

rust 如果不进 DMA 无法“舒舒坦坦”地使用api（如果你觉得拷贝源码而不是调用库算是正常使用方法那你牛逼）

M佬向原内核维护人员申请包装一层使用被拒，申请自己实现并维护一套rust的等同C的实现被骂“绝不会允许其他语言进入内核，那就是癌症”

Linus扯皮了两周未对此事发表任何意见，然后M佬怒把此事丢进舆论，他出来对M佬说，现在的问题不是对错而是你，之前已经在跑的东西能跑就是能跑，你说的对与错无所谓，你把这事儿丢舆论漩涡就是你的锅。

M佬怒辞…

—— 来自 [S1Fun](https://s1fun.koalcat.com)


*****

####  HariSeldon  
##### 92#       发表于 2025-2-12 21:11

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67401049&amp;ptid=2245923" target="_blank">abcxiawei 发表于 2025-2-12 11:16</a>
又是这套“我头脑比你强”逻辑。

我自己也是程序员出身的。我已经不止一次看到你们这种逻辑了，越年轻的 ...</blockquote>
俺寻思这个错误理解很早就被说过了。Rust语言特性多并不能推导出心智负担比C/C++重

反直觉的是，C/C++才是对程序员门槛要求高，心智负担重的那个。学习C++门槛低，靠C++吃饭门槛可高了。即使是精英程序员，精力不济时照样可能犯低级错误。而Rust的编译器检查则极大减少了业务逻辑外犯错的可能性。

一个需要用到非GC语言的非嵌入式项目，几个资深带一群普通程序员用Rust是可以干的：定好规矩or脚本检查普通程序员不可提交unsafe代码就行了，剩下自有编译器教。同样配置的团队用c++的话，不会以为编译器放行是降低心智负担吧？

至于市面上九成以上不需要非gc语言的工作…也不用关心rust，哪有那么多写rust的

— from [S1 Next Goose](https://www.pgyer.com/GcUxKd4w) v3.3.96


*****

####  coyove  
##### 93#       发表于 2025-2-12 22:42

可以去看看hellwig的回复，“不是说我不喜欢rust”，叠甲叠满<img src="https://static.saraba1st.com/image/smiley/face2017/046.png" referrerpolicy="no-referrer">，rust不愧是编程界原神


*****

####  YoumuChan  
##### 94#       发表于 2025-2-13 00:46

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67403526&amp;ptid=2245923" target="_blank">Steel.Haze 发表于 2025-2-12 16:27</a>

你这个说法太理中客。且不说换内核的整体工程代价。这种集中化模式其实增加易于被几种攻击的点而已。你只 ...</blockquote>
“由于把会出问题的地方集中起来导致容易被集中攻击”这个说法，有一种“练了金钟罩铁布衫只剩两三个罩门导致容易被集中攻击所以不如不练”的美感。

操作系统方面的落地了的应用案例有[https://github.com/cloud-hypervisor/cloud-hypervisor](https://github.com/cloud-hypervisor/cloud-hypervisor)，还有就是Asahi Linux上的GPU驱动吧。


*****

####  123485k  
##### 95#       发表于 2025-2-13 01:12

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67401866&amp;ptid=2245923" target="_blank">bcxzzz 发表于 2025-2-12 13:03</a>
对于这种后出来的语言，美国的棱镜计划之类的，会不会直接在编译器里埋后门？

—— 来自 HUAWEI LIO-AL0 ...</blockquote>
还是有可能的，可以参考[这篇博客](https://bojieli.com/2014/11/insert-backdoor-into-compiler/)


*****

####  bcxzzz  
##### 96#       发表于 2025-2-13 01:39

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67406860&amp;ptid=2245923" target="_blank">123485k 发表于 2025-2-13 01:12</a>
还是有可能的，可以参考这篇博客</blockquote>
看了这个博客，我感觉美国一直在往种操作系统里塞后门。即使用R，也要看到这个语言的源码才行。

—— 来自 HUAWEI LIO-AL00, Android 12上的 [S1Next-鹅版](https://github.com/ykrank/S1-Next/releases) v2.5.4


*****

####  御坂MKII  
##### 97#       发表于 2025-2-13 02:16

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67403275&amp;ptid=2245923" target="_blank">woodey 发表于 2025-2-12 15:58</a>

我知道rust很好，那为啥不用rust新做一个系统或者其他大型应用？而是一直依托于C/C++社区的东西 ...</blockquote>
那不是还因为之前没有更合适的，所以有丰富的历史厚重
[https://github.com/tikv/tikv](https://github.com/tikv/tikv)
[https://github.com/databendlabs/databend](https://github.com/databendlabs/databend)

数据库因为有单机转 raft/paxos based 以及未来更激进的 cloud infra 的需要，所以活跃的新项目是很多的


*****

####  gawain  
##### 98#       发表于 2025-2-13 03:14

 本帖最后由 gawain 于 2025-2-13 03:16 编辑 

这事锅就在Linus自己身上，要又不全要。 事实上今天哪怕不是rust，换任何语言都会造成社区的分裂。 本来大家都是用C。不管是维护自己的模块，还是处理其他模块的调用产生的问题。都不存在语言层面知识的障碍。现在内核引入了另一种语言的模块。那我遇到这些模块的问题，是不是还要先学会这种语言？我本来写C写的好好的。 凭啥让我学一个新语言，而且还得比较深入的研究。

[论坛助手,iPhone](https://bbs.saraba1st.com/2b/forum.php?mod=viewthread&amp;tid=2029836)


*****

####  星空天神  
##### 99#       发表于 2025-2-13 08:00

没有写过rust，不过rust既然用所有权的问题解决内存安全问题那么多线程下的内存安全是怎么在编译时期解决的？


*****

####  Xerxes_2  
##### 100#       发表于 2025-2-13 12:42

 本帖最后由 Xerxes_2 于 2025-2-13 12:46 编辑 
<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67407344&amp;ptid=2245923" target="_blank">星空天神 发表于 2025-2-13 08:00</a>

没有写过rust，不过rust既然用所有权的问题解决内存安全问题那么多线程下的内存安全是怎么在编译时期解决的 ...</blockquote>
看 Sync 和 Send 两个 trait，简单说严格限制了对象在线程之间发送/共享的要求

就我体验来说 Rust 写多线程是比 C 要方便且安全的多的（没用过 C++）


*****

####  星空天神  
##### 101#       发表于 2025-2-13 13:46

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67409925&amp;ptid=2245923" target="_blank">Xerxes_2 发表于 2025-2-13 12:42</a>

看 Sync 和 Send 两个 trait，简单说严格限制了对象在线程之间发送/共享的要求

就我体验来说 Rust 写多线 ...</blockquote>
看了一下c++大概是这么写 std::string a;     std::mutex m;     std::thread t1([&amp;]                 {                      std::lock_guard&lt;std::mutex&gt; lock(m);                     a += "hello";                  });     std::thread t2([&amp;]                 {                      std::lock_guard&lt;std::mutex&gt; lock(m);                     a += "world";                  });     t1.join();     t2.join();     std::cout &lt;&lt; a &lt;&lt; std::endl;复制代码rust要arc包裹mutex包裹string。有个疑问就是假如一个被共享的只读对象也要用arc来访问，在跨numa的情况下原子操作的代价非常昂贵，rust是如何去解决这个问题的？


*****

####  YoumuChan  
##### 102#       发表于 2025-2-13 14:10

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67410608&amp;ptid=2245923" target="_blank">星空天神 发表于 2025-2-13 13:46</a>
看了一下c++大概是这么写

rust要arc包裹mutex包裹string。有个疑问就是假如一个被共享的只读对象也要用ar ...</blockquote>
假如你在线程运行期间对共享对象不会进行更改的话，可以开scoped thread，然后直接共享只读引用就行了。编译器在发现这段生命周期里共享对象只会派生只读引用的话，就会允许你在线程间传递只读引用，所以可以不用arc，甚至不用加锁。

假如需要更改但是你可以保证线程不会后台一直运行，也即你共享的对象最终由主线程释放（持有所有权），而不会由子线程一直持有引用的话，你也可以scoped thread然后直接传递互斥锁mutex的引用，不用arc。

如果什么都不能保证，那你必然需要一个线程安全的类似shared_ptr的东西，那这个东西在rust就叫做arc。

— from [S1 Next Goose](https://www.pgyer.com/GcUxKd4w) v3.3.96


*****

####  燕山雪  
##### 103#       发表于 2025-2-13 14:23

新来者要融入高活跃度的社区，肯定要先适应已有的习惯和文化，而不是要求老屁股改变自己去讨你开心。如果需要包一层c接口，由rust人自己写好了直接请求合入，对其他人无感，可能冲突会少一些？


*****

####  d2loader  
##### 104#       发表于 2025-2-13 15:44

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67410977&amp;ptid=2245923" target="_blank">燕山雪 发表于 2025-2-13 14:23</a>
新来者要融入高活跃度的社区，肯定要先适应已有的习惯和文化，而不是要求老屁股改变自己去讨你开心。如果需 ...</blockquote>
你说的对，的确就是rust的人自己写了dma相关绑定

但是dma的老大说他要一个人审查所有dma相关的代码，rust这边自己写的绑定他看不懂，然后说这种引入第二语言的行为是癌症

之后楼主说到那位选择发到社交网络上施压

Linus对这种想要网暴的行为严厉批评

时间线是这样的

—— 来自 [鹅球](https://www.pgyer.com/GcUxKd4w) v3.3.96


*****

####  优秀  
##### 105#       发表于 2025-2-13 16:04

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67405274&amp;ptid=2245923" target="_blank">darklinden 发表于 2025-2-12 20:19</a>

他们只是想骂 rust 而已 

这事儿吧…</blockquote>
由你描述的过程看来，早前linus让rust进内核说明他也不反感rust，但下面吵了两周他没表态说明他也不知道这个问题上支持哪边好，然后rust那边把这个问题放到社交媒体上这个行为激怒了他（他觉着这种吵架就该在技术社区吵？），这时候他出来说的不是谁对而是谁错了。

好像linus这么处理也没错，当然人跑了从大局上来看是自己损失了。

*****

####  FeteFete  
##### 106#       发表于 2025-2-13 16:07

<blockquote>我是蓝石头 发表于 2025-2-12 18:10
建议python，一个上午就可以用pytorch零到一写一个简单的有监督机器学习训练加推理，感受朴素的机器学习 ...</blockquote>
写python 和写c++真的不是一个难度，哪怕写一个玩具都不一样


*****

####  darklinden  
##### 107#       发表于 2025-2-13 16:19

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67412006&amp;ptid=2245923" target="_blank">优秀 发表于 2025-2-13 16:04</a>

由你描述的过程看来，早前linus让rust进内核说明他也不反感rust，但下面吵了两周他没表态说明他也不知道 ...</blockquote>
换位思考，想象一下：

你是team leader，有一只鲶鱼进入了你的队伍，能力出众，然后有一个看起来不错的想法，进队就开始砸天花板开天窗，甚至所有工作都已经做好了（就差合并了

但是你组里的老人开始发难，说，既然老项目在跑就不要去动它，新的东西可能很好也可能引起更多的问题，甚至可能把家炸了

虽然你的直觉告诉你鲶鱼们的主张是对的，但是你一怕真炸了，二怕老人撂挑子，只好看他们打嘴仗

这时老人开始嘴臭，鲶鱼找自己要说法...

也不能开了啊，开了没人干活儿了，先晾晾？

鲶鱼被晾久了直接把嘴臭挂微博，老人开始被网暴...

烦死了，怎么还有微博挂人的家伙...先骂一顿...

艹，微博挂人那个怎么跑了?...

（HackNews还是有大批人吐槽Linus已经老了的，真换位思考一下，很多情况是管理问题造成的...吧...


*****

####  Jet.Black  
##### 108#       发表于 2025-2-13 16:24

极端反C++也是管理问题，与C兼容性最好的肯定是C++，C的高人多少也会点C++。

*****

####  优秀  
##### 109#       发表于 2025-2-13 16:29

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67412204&amp;ptid=2245923" target="_blank">Jet.Black 发表于 2025-2-13 16:24</a>

极端反C++也是管理问题，与C兼容性最好的肯定是C++，C的高人多少也会点C++。 ...</blockquote>
没学过rust，但c++编译出来的东西确实比臃肿不少，内核还是要追求小、快，操作系统内核开发用c是有道理的。


*****

####  gammatau  
##### 110#       发表于 2025-2-13 16:33

<blockquote>优秀 发表于 2025-2-13 16:04
由你描述的过程看来，早前linus让rust进内核说明他也不反感rust，但下面吵了两周他没表态说明他也不知道 ...</blockquote>
只能说一开始看错了人找了个喜欢上社交媒体闹事的，幸好他自己跑了，算止损。


*****

####  Midnight.Coup  
##### 111#       发表于 2025-2-13 17:38

 本帖最后由 Midnight.Coup 于 2025-2-13 17:41 编辑 

有人在 Linux 内核中提交了一个补丁，目的是让 Rust 编写的驱动程序能使用 dma_alloc_coherent() 函数，这样 Rust 驱动程序也能像 C 语言编写的驱动程序一样，使用 Linux 内核提供的 DMA 功能，从而更高效地处理设备与内存之间的数据传输。

然而，这个提议遭到了 Linux 内核维护者 Christoph Hellwig 的强烈反对。Hellwig 明确表示，他不希望在内核的 DMA 部分看到 Rust 代码。实际上，这个补丁只是将代码添加到了一个不同的地方（rust/kernel），而不是直接改动 DMA （kernel/dma）部分。

Hellwig 的拒绝让很多 Rust 开发者们感到郁闷，对此，Rust for Linux 项目的首席开发者 Miguel Ojeda 出面请求 Hellwig 给出一个替代方案。Hellwig 回应道：“把包装器放在你们自己的代码里，而不是让别人为你们的事情受苦。”

因为是在邮件列表的回应，所有开发者都可以看到，对此，Red Hat 的软件工程师 Danilo Krummrich 直接质问 Hellwig，“你们自己的代码是什么意思？是不是在每个驱动程序中都重复了？否则，rust/kernel/dma.rs 看起来合理，对吧？”

Hellwig 接着表示：“DMA API 的接口应该保持在可读的 C 代码中，而不是用奇怪的绑定来实现，这样它才可以被 grep 搜索并且更易于维护。”

此外，Hellwig 也明确表示他根本不愿意处理 Rust 代码。他写道：“不要强迫我处理你们这门时髦的语言。维护多语言的项目很痛苦，我没有兴趣去处理。如果你们想用的不是 C 语言，像汇编语言或 Rust，你们自己写 C 接口，自己解决语言不匹配的问题，反正我不管。”

Red Hat 的软件工程师 Danilo Krummrich 解释称，并没有人要求你处理或者维护这段 Rust 代码。Rust for Linux 项目正在创建 Rust 代码，它将 C API 抽象化，供所有 Rust 驱动程序使用，并由 Rust 开发者来维护。

换句话说，内核中的 C 代码保持不变，而 Rust 驱动程序通过抽象层来使用这些 C 代码，这些抽象层由 rust/kernel 中的团队集中维护，整体上比每个驱动程序自己编写 C 语言绑定要好。

但 Hellwig 似乎不愿意让 DMA 的 Rust 抽象层单独维护，甚至不应该在 Linux 源代码树 rust/kernel 中维护。他怒斥道：“如果你们想让 Linux 因为跨语言的代码库变得无法维护，那就让你们的驱动自己去做吧，而不是把这种‘癌症’传播到核心子系统中。”

Hellwig 继续论述说，让其他人单独维护 Rust 的抽象层来处理 DMA 的内存分配器，并不会改善问题，反而会妨碍内核的可维护性：“每引入一种新语言，就会**降低内核作为一个整体项目的可维护性。Linux 之所以能生存这么久，是因为它没有内部边界，而引入另一种语言完全破坏了这一点。你可能不喜欢我这么说，但我会尽全力阻止这种做法。这不是因为我讨厌Rust。虽然它不是我最喜欢的语言，但它绝对是新兴语言中最好的之一，我鼓励人们在适合的情况下用于新项目。我只是不希望它出现在我需要维护的大型 C 语言代码库中。”

几轮辩论之后，Red Hat 的软件工程师 Danilo Krummrich 认为 Hellwig 作为一名维护者，他的一些举措超出了维护者的工作范围，即：根据个人喜好，任意限制某个实体对公共内核 API 的使用。

为此，他和 Asahi Linux 项目负责人 Hector Martin 纷纷请求 Linux 之父 Linus Torvalds 出面解决这一问题。

Asahi Linux 项目负责人 Hector Martin 在邮件中写道： <blockquote>我的看法：如果 Linus 没有在这个讨论中给出权威的答复，Miguel 和其他 Rust 的开发者应该在代码经过审查并准备好后，直接合并这部分内容，不必理会 Christoph Hellwig 明显想要破坏项目的行为。

如果 Linus 拒绝合并，那么 Christoph 说的就无关紧要了。

如果 Linus 不合并，R4L 项目基本上就会死掉，除非 Linus 或 Christoph 采取行动。其他的讨论只是绕圈子。

Rust 开发者们：请不要浪费时间和精力去纠结这种戏剧性的事情，这不值得。要么 Linus 喜欢，要么他不喜欢。其他的都是少数破坏者维护者故意制造的干扰，他们想通过打击你们的士气来让你们放弃，因为他们知道自己终究会在历史中处于失败的一方。旧的固守阵地的维护者再怎么破坏，也无法阻止世界向内存安全语言的方向发展。

顺便说一句，我认为 Christoph 的“癌症”言论足以成为违反行为规范的理由，但我怀疑不会有任何相应的处理。</blockquote>
殊不知，Hector Martin 的这一则邮件直接将 Linus 推到需要做出二选一决策的”边缘“。

面对 Hector Martin 呼吁 Linus “发表权威回答”以解决设备驱动的僵局，并支持通过“社交媒体羞辱”来反击 Linux 维护者对 Rust 代码的敌视，Linus 对此方法予以否定。

Linus 极其礼貌但毫不客气地回应 Martin： <blockquote>Martin：如果在社交媒体上羞辱他人没有效果，那就告诉我，还有什么方法有效，因为我已经没有其他办法了。

你能不能接受一个事实，也许问题出在你自己身上？

你以为你知道得更好，但目前的流程是有效的。

它有问题，但问题是生活的一部分。没有完美的东西。

不过，我必须说，社交媒体的“围攻”让我根本不想再和你们的做法有任何关系。

因为如果我们在内核开发模式中有问题，那么社交媒体绝对不是解决方案。就像它根本不是政治问题的解决方案一样。

技术补丁和讨论才是关键。社交媒体围攻——谢谢，但不需要。</blockquote>

在得到 Linus 的回复之后，Hector Martin 愤而决定辞去 Apple Silicon 代码的上游维护者职务。

Hector Martin 在最新的一次补丁中写道：“我已经不再对内核开发过程或社区管理方式抱有任何信心。Apple/ARM 平台的开发将继续在下游进行。如果未来我有兴趣向上游提交一些补丁，不管是针对哪个子树，我可能会，也可能不会。任何愿意自己为上游提交做出努力的人都可以去做。”

Asahi Linux 的开发者兼共同维护者 Sven Peter 听闻这一消息后出面表示：“给我几天时间来弄清楚我们该怎么做。我认为我们可以继续推动该树的前进。”

在引入 Rust 的过程中，C 和 Rust 开发者之间的摩擦也是不可避免的，Linux 的创始人 Linus Torvalds 也对此有深刻认识，他曾在 Linux 基金会的开放源代码峰会上提到过这一点。

Torvalds 说：“显然，有些人就是不喜欢 Rust，也不希望 Rust 侵犯他们的领域。有人甚至在说 Rust 的整合是失败的……我们做这个已经好几年了，现在说失败还太早，但即使它最终失败了——虽然我不认为会失败——那也是一种学习的方式。”

此外，他还指出，目前内核中的任何功能都不依赖 Rust，短期内也不会依赖。重要的是向前推进，因此开发者们应该“全速前进”，暂时不要太在意这些问题。即便现在细节还不完善，只要能让功能正常运行就足够了。一旦用户开始依赖 Rust 代码，才需要更细致地处理这些问题。但现在，如果开发者因为过于谨慎而裹足不前，反而会让项目受挫。

只是在此次争论中，Linus 的处理方式让不少开发者觉得有些不满： <blockquote>Rust 问题暴露了 Torvalds 作为领导者的一次罕见失职。与其果断地说“不是，绝对不行”或者“是的，执行”，他在 Rust 的问题上一直模棱两可。

鉴于 Linux 社区中有相当一部分（且非常 vocal）的人对他的决定产生了信任危机，这种犹豫不决的态度反而起到了适得其反的效果。而且 Linus 没有明确立场，实在是有些反常（比如我们都知道他对 C++ 的立场）。

作为一个试点项目，R4L 应该早就毕业或者结束了。但经过多年积极开发，它的现状依旧不明朗。Linus 并没有采取措施让大家达成共识，而是选择一直坐视不管，看着下属们相互争斗，最后还将责任推给 Martin，实在是欠妥。

可以说，他对 Martin 的训斥明显表明了他永远不会偏袒 Rust，但他并没有明确说出来。也许他知道应该表态，但又担心会引发一场风暴。也许现在是时候撕掉创可贴了。

再说一次，所有这些本来都可以避免，如果他当初能坚定地站队，不论是赞成还是反对。想象一下，如果 Linus 直接说“不要，保持在下游”，能节省多少时间和精力，甚至是仅仅 Martin 的时间。</blockquote>


*****

####  Xerxes_2  
##### 112#       发表于 2025-2-13 17:46

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67413034&amp;ptid=2245923" target="_blank">Midnight.Coup 发表于 2025-2-13 17:38</a>

有人在 Linux 内核中提交了一个补丁，目的是让 Rust 编写的驱动程序能使用 dma_alloc_coherent() 函数，这 ...</blockquote>
Asahi Linux 的图形驱动似乎就是 Rust 的


*****

####  Midnight.Coup  
##### 113#       发表于 2025-2-13 17:56

 本帖最后由 Midnight.Coup 于 2025-2-13 18:00 编辑 
<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67413112&amp;ptid=2245923" target="_blank">Xerxes_2 发表于 2025-2-13 17:46</a>

Asahi Linux 的图形驱动似乎就是 Rust 的</blockquote>
Linus 本人还在 mba 上用 Asahi Linux，R4L 也是 Linus 点头进主线，就很一言难尽，这件事归根到底是 Linus 的态度不明，整双方的像后宫斗争，Linus 最后左右都不好偏，只能从态度上拿 M 佬开刀

*****

####  vail潇  
##### 114#       发表于 2025-2-13 17:56

支持rust的人再用rust重构一版不行吗？

—— 来自 vivo V2307A, Android 15上的 [S1Next-鹅版](https://github.com/ykrank/S1-Next/releases) v2.1.2

*****

####  Xerxes_2  
##### 115#       发表于 2025-2-13 17:59

 本帖最后由 Xerxes_2 于 2025-2-13 18:00 编辑 
<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67413216&amp;ptid=2245923" target="_blank">vail潇 发表于 2025-2-13 17:56</a>

支持rust的人再用rust重构一版不行吗？

—— 来自 vivo V2307A, Android 15上的 S1Next-鹅版 v2.1.2 ...</blockquote>
[https://www.redox-os.org/](https://www.redox-os.org/)

?

坛友真的有点搞笑了，一点不懂就原神原神后门后门的叫

*****

####  RookieTnT  
##### 116#       发表于 2025-2-13 18:02

字节的rsbuild 和 rspack倒是挺好用的


*****

####  Xerxes_2  
##### 117#       发表于 2025-2-13 18:05

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67413266&amp;ptid=2245923" target="_blank">RookieTnT 发表于 2025-2-13 18:02</a>

字节的rsbuild 和 rspack倒是挺好用的</blockquote>
现在开发基建用 Rust 的挺多的了，数了下我电脑上的 $brew uses rust --installed --include-build --include-implicit --include-optional                                                                                                                  aider                  fd                     hyperfine              librsvg                ripgrep                tectonic               typst                  uutils-coreutils       zoxide bat                    fish                   kondo                  mise                   scriptisto             tokei                  typstyle               uv eza                    helix                  libimagequant          rav1e                  starship               tree-sitter            usage                  yazi 复制代码


*****

####  unlsycn  
##### 118#       发表于 2025-2-13 18:33

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67413034&amp;ptid=2245923" target="_blank">Midnight.Coup 发表于 2025-2-13 17:38</a>

有人在 Linux 内核中提交了一个补丁，目的是让 Rust 编写的驱动程序能使用 dma_alloc_coherent() 函数，这 ...</blockquote>
「罕见」失职.jpg


*****

####  unlsycn  
##### 119#       发表于 2025-2-13 18:36

不知道楼里的坛友是怎么一口一个「HaskWell」还有信心装PL大手子的<img src="https://static.saraba1st.com/image/smiley/face2017/076.png" referrerpolicy="no-referrer">问就是原神.jpg


*****

####  ryanz  
##### 120#       发表于 2025-2-13 18:59

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67402158&amp;ptid=2245923" target="_blank">万恶淫猥手 发表于 2025-2-12 13:45</a>

Rust 粉和 NodeJS 粉已经快接近之前的 PHP 了

另外人家 Kernel 也没反对你用 Rust，是说你不能乱搞也给你 ...</blockquote>
别瞎说，现在的 nodejs 粉大概确实消散完了，对于这些争论只能说时间证明一切吧<img src="https://static.saraba1st.com/image/smiley/face2017/044.png" referrerpolicy="no-referrer">

说到时间，最近 10 年的新生代语言我就喜欢 zig，相对其他次生代语言 比如 golang 的 cgo 以及 rust 的 bindgen 引用 c 库的方式，它干净太多。这里还是要吐槽下 rust，bindgen 出来的东西编译后 strip 不干净，导致执行文件体积**增加<img src="https://static.saraba1st.com/image/smiley/face2017/022.png" referrerpolicy="no-referrer">


*****

####  darklinden  
##### 121#       发表于 2025-2-13 19:58

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67413760&amp;ptid=2245923" target="_blank">ryanz 发表于 2025-2-13 18:59</a>
别瞎说，现在的 nodejs 粉大概确实消散完了，对于这些争论只能说时间证明一切吧

说到时间，最近 10 年的 ...</blockquote>
请问对于zig编写的bun存在各种奇特内存泄漏的问题怎么看？

zig编译太好使了以至于目前最常见的时候都是在干编译的活儿…

<img src="https://static.saraba1st.com/image/smiley/face2017/004.gif" referrerpolicy="no-referrer">

—— 来自 [S1Fun](https://s1fun.koalcat.com)


*****

####  d2loader  
##### 122#       发表于 2025-2-13 20:05

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67414230&amp;ptid=2245923" target="_blank">darklinden 发表于 2025-2-13 19:58</a>
请问对于zig编写的bun存在各种奇特内存泄漏的问题怎么看？

zig编译太好使了以至于目前最常见的时候都是 ...</blockquote>
zig可能靠这个这个独门绝活活下去的

希望rust这边早点造好allocator-api 2

—— 来自 [鹅球](https://www.pgyer.com/GcUxKd4w) v3.3.96


*****

####  GJRstone  
##### 123#       发表于 2025-2-13 20:39

一切皆政治，世界最大的开源运动皇冠上的明珠linux内核实际上就是靠林纳斯这个象征从外围凝聚起来的，在林纳斯通过秘密集会认定一部分俄罗斯开发者是敌我关系并依托美国法律对这些人进行政治迫害时，linux社区在二十年尺度上发生分裂的不确定性肯定会增加。

而林纳斯客观来说55岁，说长寿能活20年，那么他自然需要考虑权力交接的问题。延续c/c++，是继续把心智负担叠加在管理者上，引入rust，是把心智负担解放到一部分rust贡献者头上——或者更具体的说rust委员会头上。
往下有几层问题：①rust委员会的稳定性②作为某一个特定象征发生时，c/c++开发者缺乏核心领导散兵游勇而rust开发者作为尖刀部队显著夺权造成生态动荡的可能性。

社交媒体逼宫毫无疑问是②的风险发生的指示物，而rust委员会在23年重组本身就说明rust“命不久矣”。林纳斯55岁不是75岁，身后还有c++委员会（除社区支持外还特指美国政府那部分影子）撑腰，肯定不会鸟rust的逼宫行为。


*****

####  yikaa  
##### 124#       发表于 2025-2-13 20:49

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67404297&amp;ptid=2245923" target="_blank">bcxzzz 发表于 2025-2-12 18:02</a>
从技术上来说，可能给一种语言留后门么？ 比如考虑下：1、语言的解释器、编译器是公开代码的么？ 2，即使 ...</blockquote>
https://wiki.c2.com/?TheKenThompsonHack

如果仅说有没可能，那是有可能的

—— 来自 [鹅球](https://www.pgyer.com/GcUxKd4w) v3.3.96


*****

####  ryanz  
##### 125#       发表于 2025-2-13 21:15

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67414230&amp;ptid=2245923" target="_blank">darklinden 发表于 2025-2-13 19:58</a>

请问对于zig编写的bun存在各种奇特内存泄漏的问题怎么看？

zig编译太好使了以至于目前最常见的时候都是 ...</blockquote>
选择工具比较保守就没用过，写前端还是 vite react 默认的那套脚手架。我感觉是最近两三年的东西吧，年轻的应用有各种问题很正常，就像当初 swc 和 esbuild 运行效率导致的那些争论，前期没优化完全并不足以说明什么。


*****

####  万恶淫猥手  
##### 126#       发表于 2025-2-13 21:32

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67414230&amp;ptid=2245923" target="_blank">darklinden 发表于 2025-2-13 19:58</a>

请问对于zig编写的bun存在各种奇特内存泄漏的问题怎么看？

zig编译太好使了以至于目前最常见的时候都是 ...</blockquote>
zig 本身就是显示管理的，写着写着就忘属于老问题了…


*****

####  星空天神  
##### 127#       发表于 2025-2-13 23:18

以后都是ai的世界,编程语言算个球<img src="https://static.saraba1st.com/image/smiley/face2017/037.png" referrerpolicy="no-referrer">


*****

####  星空天神  
##### 127#       发表于 2025-2-13 23:18

以后都是ai的世界,编程语言算个球<img src="https://static.saraba1st.com/image/smiley/face2017/037.png" referrerpolicy="no-referrer">

*****

####  Midnight.Coup  
##### 128#       发表于 2025-2-17 16:22

Hector "marcan" Martin 宣布辞去 Asahi Linux 项目负责人的职务
[https://marcan.st/2025/02/resigning-as-asahi-linux-project-lead/](https://marcan.st/2025/02/resigning-as-asahi-linux-project-lead/)


*****

####  UNICORN00  
##### 129#       发表于 2025-2-18 00:51

唉

—— 来自 [鹅球](https://www.pgyer.com/GcUxKd4w) v3.3.96

