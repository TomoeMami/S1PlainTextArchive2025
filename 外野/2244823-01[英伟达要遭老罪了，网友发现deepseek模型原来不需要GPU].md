
*****

####  宏.  
##### 1#       楼主       发表于 2025-2-1 00:27

 本帖最后由 宏. 于 2025-2-1 00:28 编辑 

简单来说，直接用大内存+多块SSD就可以跑671B（全尺寸）deepseek R1模型，根本不用GPU，这要是确实可行，LLM直接变成小算力+大存储模式，这甚至能塞进笔记本里面，谁还需要买老黄的GPU，英伟达腰斩指日可待<img src="https://static.saraba1st.com/image/smiley/face2017/037.png" referrerpolicy="no-referrer">直觉上这确实更接近人脑的模型

[https://www.reddit.com/r/LocalLL ... sec_without_gpu_on/](https://www.reddit.com/r/LocalLLaMA/comments/1idseqb/deepseek_r1_671b_over_2_toksec_without_gpu_on/)

<img src="https://img.saraba1st.com/forum/202502/01/002757stoleobelemo4s55.png" referrerpolicy="no-referrer">

<strong>Snipaste_2025-02-01_00-21-32.png</strong> (247.52 KB, 下载次数: 0)

下载附件

2025-2-1 00:27 上传

﹍﹍﹍

评分

 参与人数 1战斗力 +1

|昵称|战斗力|理由|
|----|---|---|
| 偽物| + 1|好评加鹅|

查看全部评分

*****

####  希望之花  
##### 2#       发表于 2025-2-1 00:29

记得一开始还要用英伟达自家的汇编，现在已经迭代到不用gpu了吗<img src="https://static.saraba1st.com/image/smiley/face2017/068.png" referrerpolicy="no-referrer">

----发送自 [STAGE1 App for Android.](http://stage1.5j4m.com/?1.44)

*****

####  a317216007  
##### 3#       发表于 2025-2-1 00:29

<img src="https://static.saraba1st.com/image/smiley/face2017/018.png" referrerpolicy="no-referrer">把配置要求摸清楚的话，堆一堆内存和SSD说不定能整一个一键部署的家庭装

﹍﹍﹍

评分

 参与人数 1战斗力 +1

|昵称|战斗力|理由|
|----|---|---|
| 偽物| + 1|好评加鹅|

查看全部评分

*****

####  cnwind042  
##### 4#       发表于 2025-2-1 00:32

烧GPU算力的不是训练的时候吗，部署本来也不会给老黄多卖多少GPU吧<img src="https://static.saraba1st.com/image/smiley/face2017/180.png" referrerpolicy="no-referrer">

*****

####  qumkml423  
##### 5#       发表于 2025-2-1 00:35

那利好有海力士三星的棒子了

*****

####  树洞专用  
##### 6#       发表于 2025-2-1 00:36

跑完整模型真的牛逼好吧，观望一下r2出来能不能这么玩，说不定得提前囤点固态，比h100可便宜多了

*****

####  璇瑢子R  
##### 7#       发表于 2025-2-1 00:38

本来都可以用cpu跑呀。只要你能存的下运行的模型

*****

####  jxwats1  
##### 8#       发表于 2025-2-1 00:41

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67324590&amp;ptid=2244823" target="_blank">希望之花 发表于 2025-2-1 00:29</a>
记得一开始还要用英伟达自家的汇编，现在已经迭代到不用gpu了吗

----发送自 STAGE1 App for Android. ...</blockquote>
不一样，你说的是训练的时候没用coda，这里是用训练好的模型推理不用显卡

*****

####  frankCC  
##### 9#       发表于 2025-2-1 00:41

你看下帖子内容啊，每秒 2token 的输出黄花菜都凉了，这帖子纯粹为了迎合反老黄的情绪，一点实用性都没有。

*****

####  d2loader  
##### 10#       发表于 2025-2-1 00:41

 本帖最后由 d2loader 于 2025-2-1 00:42 编辑 

AMD狂喜，你这个思路不如双路epyc吃满24通道DDR5跑了

国外已经有人做过试验能跑到8tokens每秒

—— 来自 [鹅球](https://www.pgyer.com/GcUxKd4w) v3.3.96

*****

####  宏.  
##### 11#         楼主| 发表于 2025-2-1 00:42

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67324634&amp;ptid=2244823" target="_blank">璇瑢子R 发表于 2025-2-1 00:38</a>

本来都可以用cpu跑呀。只要你能存的下运行的模型</blockquote>
deepseek以前CPU跑的效率是没法接受的，但这要是真行，瓶颈在pcie通道上

*****

####  alixsander  
##### 12#       发表于 2025-2-1 00:44

2tps什么概念，兄弟

不要搞笑好吗

*****

####  璇瑢子R  
##### 13#       发表于 2025-2-1 00:46

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67324624&amp;ptid=2244823" target="_blank">qumkml423 发表于 2025-2-1 00:35</a>
那利好有海力士三星的棒子了</blockquote>
主贴里这个人用ssd只是因为他只有96G内存。装不下整个模型
只要内存够大就完全不需要和ssd有关

*****

####  宏.  
##### 14#         楼主| 发表于 2025-2-1 00:46

 本帖最后由 宏. 于 2025-2-1 00:50 编辑 
<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67324641&amp;ptid=2244823" target="_blank">frankCC 发表于 2025-2-1 00:41</a>

你看下帖子内容啊，每秒 2token 的输出黄花菜都凉了，这帖子纯粹为了迎合反老黄的情绪，一点实用性都没有。 ...</blockquote>
你仔细看，这是x4 nvme跑出来的，这才16x通道，家用机主板专门设计一下搞个64x，插16个ssd问题不大

*****

####  tansapple  
##### 15#       发表于 2025-2-1 00:46

好消息是显卡还能继续探底，坏消息是固态要涨了是吗？<img src="https://static.saraba1st.com/image/smiley/face2017/067.png" referrerpolicy="no-referrer">

*****

####  凉良  
##### 16#       发表于 2025-2-1 00:46

这么高配置结果每秒2token  只能说闹麻了

*****

####  都是好事  
##### 17#       发表于 2025-2-1 00:49

不是一直可以吗？用gpu是快

*****

####  坏掉了  
##### 18#       发表于 2025-2-1 00:51

还是需要大内存，4xNVMe的速度不行

*****

####  宏.  
##### 19#         楼主| 发表于 2025-2-1 00:52

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67324671&amp;ptid=2244823" target="_blank">凉良 发表于 2025-2-1 00:46</a>

这么高配置结果每秒2token  只能说闹麻了</blockquote>
看原文。这个速度的瓶颈根本不在CPU和GPU，30901ti纯粹是个摆设

After experimenting with various setups, the bottle neck is clearly my Gen 5 x4 NVMe SSD card as the CPU doesn't go over ~30%, the GPU was basically idle, and the power supply fan doesn't even come on.

*****

####  tonyunreal  
##### 20#       发表于 2025-2-1 00:52

6000刀买epyc或者Mac Studio(m2 ultra)的方案更可行一点

—— 来自 [鹅球](https://www.pgyer.com/GcUxKd4w) v3.3.96

*****

####  Alce79  
##### 21#       发表于 2025-2-1 00:52

 本帖最后由 Alce79 于 2025-2-1 00:54 编辑 

这次的事对老黄是绝对利好，轻量化用户吃不着但是能吃上各国的ai梦. 英国国会上也开始讨论建设ai了.

BV1NTFDe3EQ2

沙特肯定也会跟上，打下价格之后会掀起ai狂潮.

除了基础通用模型以外还有各家公司给用户打造的专用模型（类似tiktok算法怎么舒服怎么来）.

最惨的只有奥特曼和闭源门阀，要么抓紧跑出划时代Ai要么开源大家一起滚泥巴.

*****

####  lin2004  
##### 22#       发表于 2025-2-1 00:53

<blockquote>坏掉了 发表于 2025-2-1 00:51
还是需要大内存，4xNVMe的速度不行</blockquote>
该出专用硬件了.PNG

*****

####  catyoursis  
##### 23#       发表于 2025-2-1 00:56

这个文的意思大概是对于一般人来说，用显卡跑部署好的蒸馏模型，不如直接用4块nvme ssd来跑671B的完整模型，他意思是虽然慢，但是质量比蒸馏的好。

不过2tps是不是太慢了。。

*****

####  百猪夜行  
##### 24#       发表于 2025-2-1 00:56

我机器是64g内存加4090，跑32b那个能全装显存里非常快，跑70b那个内存虽然能装的下，但速度就慢了不少。如果是完整671b那个模型，内存都装不下跑在SSD上速度会慢的没有实用价值吧。

—— 来自 [鹅球](https://www.pgyer.com/xfPejhuq) v3.3.96-alpha

*****

####  lin2004  
##### 25#       发表于 2025-2-1 01:00

<blockquote>百猪夜行 发表于 2025-2-1 00:56
我机器是64g内存加4090，跑32b那个能全装显存里非常快，跑70b那个内存虽然能装的下，但速度就慢了不少。如 ...</blockquote>
还是有意义的，单人跑着玩只要求10到20每秒的话瓶颈在hbm上，有人搞特化硬件的话完整模型作为个人玩具可就有盼头了。

*****

####  LeonsCat  
##### 26#       发表于 2025-2-1 01:10

那啥，你敲算盘、列竖式手撸算子也能跑，连CPU都不需要。

*****

####  宏.  
##### 27#         楼主| 发表于 2025-2-1 01:11

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67324726&amp;ptid=2244823" target="_blank">lin2004 发表于 2025-2-1 01:00</a>

还是有意义的，单人跑着玩只要求10到20每秒的话瓶颈在hbm上，有人搞特化硬件的话完整模型作为个人玩具可 ...</blockquote>
对，这个案例实际是说CPU/GPU就不是本地运行的瓶颈，瓶颈是在满足足够存储容量之后的存储带宽，显然用显存是太贵了而且老黄压根不卖给你，用内存也很贵，用SSD很便宜但是很慢，那么问题变成了用什么样的存储组合能跑出来20token的速度

*****

####  liquer  
##### 28#       发表于 2025-2-1 01:13

这会不会利好asic

*****

####  冰寒之月  
##### 29#       发表于 2025-2-1 01:16

ssd还是太慢了 普通内存其实就够了 利好EPYC

AMD Yes！

*****

####  月亮上的珊瑚  
##### 30#       发表于 2025-2-1 01:18

这是不是有利于推进PCIe7.0

*****

####  qwased  
##### 31#       发表于 2025-2-1 01:23

 本帖最后由 qwased 于 2025-2-1 01:26 编辑 

<img src="https://static.saraba1st.com/image/smiley/face2017/050.png" referrerpolicy="no-referrer">你去买一套华强北E5+C612神机插满768GB内存也就四千多RMB，速度也是2token/s啊

*****

####  明羽杏子  
##### 32#       发表于 2025-2-1 01:46

闹麻了，你用cpu跑跑试试

—— 来自 [鹅球](https://www.pgyer.com/GcUxKd4w) v3.3.96

*****

####  btnooni  
##### 33#       发表于 2025-2-1 01:52

<img src="https://static.saraba1st.com/image/smiley/face2017/034.png" referrerpolicy="no-referrer">我看有人拿纯EYPC+ddr5跑400GB的671B的R1也在2t/s左右，主楼那贴跑的是200G的MoE量化671B，拿来给EYPC跑那可以往4t/s靠了吧。然后这配置随便跑个70B模型那速度肯定够用。

*****

####  gammatau  
##### 34#       发表于 2025-2-1 02:16

 本帖最后由 gammatau 于 2025-2-1 02:21 编辑 

这是真烧SSD啊哥们

2bit的量化模型就200多G，上个服务器直接装256G内存不比整这SSD便宜？还更快

*****

####  Beams!  
##### 35#       发表于 2025-2-1 02:20

这个帖子应该发在弱智吧。。。

*****

####  中国科学院  
##### 36#       发表于 2025-2-1 02:26

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67324661&amp;ptid=2244823" target="_blank">alixsander 发表于 2025-2-1 00:44</a>
2tps什么概念，兄弟

不要搞笑好吗</blockquote>
那不，就是，这样，说，话的，样子，<img src="https://static.saraba1st.com/image/smiley/face2017/057.png" referrerpolicy="no-referrer">

—— 来自 [鹅球](https://www.pgyer.com/GcUxKd4w) v3.3.96

*****

####  Sza  
##### 37#       发表于 2025-2-1 02:28

 本帖最后由 Sza 于 2025-2-1 02:37 编辑 

一个想法，傲腾持久内存DCPMM性能介于内存和SSD，如果未来有（国产）厂商能以合理价格生产以及生态开放，LLM是不是能用上？

我想到这点后去查了下新闻，刚好看见新存科技在上个月发了新产品的官网新闻 <blockquote> 新存科技发布升级版更大容量存储芯片“NM102”

2025年1月22日，公司宣布最新力作——非易失性新型存储器“NM102”震撼问世。这款新产品不仅单颗芯片容量达到了惊人的128Gb，更在性能上实现了重大突破，支持4K高速访问，读带宽高达3.2GB/s，树立了业界新标杆。

<img src="https://img.saraba1st.com/forum/202502/01/023705g8axcs0kd82lfduz.png" referrerpolicy="no-referrer">

<strong>IMG_2321.png</strong> (160.5 KB, 下载次数: 0)

下载附件

2025-2-1 02:37 上传

在实际应用场景中，“NM102”展现出了卓越的性能表现。经过严格测试，搭载该芯片的服务器能够实现微秒级的超快响应时间，确保企业在处理海量数据时，仍能保持高效流畅的运行状态。这一显著提升，对于需要处理大量数据的企业级用户而言，无疑是一大福音，能够极大地提高工作效率。

值得一提的是，“NM102”在保证高性能的同时，还采用了独特的存储机制，有效延长了存储寿命，**降低了客户的整体拥有成本。这一创新设计，不仅提升了产品的性价比，也进一步增强了新存科技在存储市场的竞争力。

此次发布的“NM102”，不仅是公司在大容量新型存储器领域的又一力作，更是技术创新和产品升级的生动体现。与2024年9月成功发布的中国首款最大容量新型存储器芯片“NM101”相比，“NM102”在容量上实现了翻倍增长，标志着新存科技在大容量存储技术上迈出了更加坚实的一步。

目前，公司已经初步构建了有竞争力的新型存储芯片产品组合，并积极向国内云服务厂商等核心客户提供“NM102”样品，进行了一系列严格的性能测试和兼容性验证。这一系列举措的顺利实施，不仅验证了“NM102”的卓越性能和稳定性，也为新存科技在未来市场中的广泛应用奠定了坚实基础。

随着大数据应用的迅猛发展，市场对高性能存储产品的需求日益增加。公司此次推出的“NM102”，恰逢其时，将助力新存科技在大数据时代浪潮中迅速占领市场制高点，为终端用户提供更加高效、可靠的存储解决方案，创造更大的价值回报。

[https://www.numemory.com/newsinfo/7985708.html](https://www.numemory.com/newsinfo/7985708.html)</blockquote>

*****

####  big9999  
##### 38#       发表于 2025-2-1 03:01

以前硬盘挖矿又可以再来一遍了？

*****

####  懂懂懂？  
##### 39#       发表于 2025-2-1 03:10

我记得ai刚火的时候就可以用cpu了

*****

####  24k纯帅  
##### 40#       发表于 2025-2-1 04:05

训练和推理本来就不是一回事，


*****

####  希德尼娅  
##### 41#       发表于 2025-2-1 04:54

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67324714&amp;ptid=2244823" target="_blank">百猪夜行 发表于 2025-2-1 00:56</a>
我机器是64g内存加4090，跑32b那个能全装显存里非常快，跑70b那个内存虽然能装的下，但速度就慢了不少。如 ...</blockquote>
32b和70b的输出差别大吗


*****

####  strider_oy  
##### 42#       发表于 2025-2-1 05:08

2 token每秒也太慢了。我看到有用raspberry pi跑到也是这个速度，不过那个是小几号的模型。

— from [S1 Next Goose](https://www.pgyer.com/GcUxKd4w) v3.3.96


*****

####  Vacuolar  
##### 43#       发表于 2025-2-1 08:30

GPU对于跑ai从来不是必须的，只是它跑最快，对于ai这种需要反复跑反复调的东西，速度很关键


*****

####  Evspeed  
##### 44#       发表于 2025-2-1 08:38

当年不批英伟达收购mellanox感觉很多问题都不会有

*****

####  百猪夜行  
##### 45#       发表于 2025-2-1 08:39

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67325050&amp;ptid=2244823" target="_blank">希德尼娅 发表于 2025-2-1 04:54</a>
32b和70b的输出差别大吗</blockquote>
差不多，区别不大，都远不如完整在线版的，比如叫它写个七言诗，它们都能理解对仗，但都理解不了平仄关系。32b的好像只能固定输出七言律诗，70b的各种形式都有。

—— 来自 [鹅球](https://www.pgyer.com/xfPejhuq) v3.3.96-alpha


*****

####  加藤樱  
##### 46#       发表于 2025-2-1 09:52

一台96G内存的mac studio应该能跑70b的模型了


*****

####  KevinGraham  
##### 47#       发表于 2025-2-1 10:17

deepaeek以前类似参数的模型cpu跑也是这个速度，deepseek是提升了600b这个量级模型的性能，对怎么跑并没有什么改变啊
最近这些新闻就突出一个以前完全没研究过怎么本地部署大模型<img src="https://static.saraba1st.com/image/smiley/face2017/037.png" referrerpolicy="no-referrer">

*****

####  張無忌  
##### 48#       发表于 2025-2-1 10:19

[https://zhuanlan.zhihu.com/p/20714478546](https://zhuanlan.zhihu.com/p/20714478546)

eypc双路不带显卡跑deepseek，速度有6-8T/S


*****

####  鱼丈人  
##### 49#       发表于 2025-2-1 10:45

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67324624&amp;ptid=2244823" target="_blank">qumkml423 发表于 2025-2-1 00:35</a>
那利好有海力士三星的棒子了</blockquote>
国内是不是没有投资韩股的渠道


*****

####  ななひら  
##### 50#       发表于 2025-2-1 10:58

感觉大家都忽略了一个问题，除了参数本身要占内存，加大上下文长度也要占很多内存。2k的上下文干不了什么活，也就演示一下，mac的统一内存目前最大也就192，很是捉襟见肘。


*****

####  FeteFete  
##### 51#       发表于 2025-2-1 11:01

闹麻了，最近这些不懂机器学习的网友随便转发的那些憨卵新闻的真的太多了

前面的ptx汇编不要cuda贴

这里的纯cpu跑推理贴

我给你们指明一个专业一点吹逼贴

官方支持vlllm加deepseek

这样你们就可以用内存补充显存了！！ 

也算是避免卡脖子 用家用gpu跑deepseek了


*****

####  FeteFete  
##### 52#       发表于 2025-2-1 11:05

在推理领域确实有人做了三级缓存系统，你甚至可以拿来把固态当第三级缓存

不过根据vllm的论文推算 较小的块甚至不如重新计算

*****

####  宏.  
##### 53#         楼主| 发表于 2025-2-1 11:07

<blockquote>KevinGraham 发表于 2025-2-1 10:17
deepaeek以前类似参数的模型cpu跑也是这个速度，deepseek是提升了600b这个量级模型的性能，对怎么跑并没有 ...</blockquote>
主要差别是本地跑60B没啥应用价值，跑600B就应用价值很大了

至于速度，2t/s是太慢了，但1000t/s也对本地个人使用完全过剩，20t/s就是目标速度了


*****

####  lin2004  
##### 54#       发表于 2025-2-1 11:16

反正现在大家刚开始玩还没摸出优化方案，蹲个啥时候能优化到家用nas一样，个人负担得起的定制硬件能家里摆一套玩完整模型跑出10到20tps就算成功


*****

####  aimbot  
##### 55#       发表于 2025-2-1 11:33

我佛，用屁股说话就是比用脑袋说话的牛逼

*****

####  CCauchy  
##### 56#       发表于 2025-2-1 11:36

傲腾？<img src="https://static.saraba1st.com/image/smiley/face2017/053.png" referrerpolicy="no-referrer">

[论坛助手,iPhone](https://bbs.saraba1st.com/2b/forum.php?mod=viewthread&amp;tid=2029836)


*****

####  sellboy  
##### 57#       发表于 2025-2-1 11:40

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67325870&amp;ptid=2244823" target="_blank">宏. 发表于 2025-2-1 11:07</a>

主要差别是本地跑60B没啥应用价值，跑600B就应用价值很大了

至于速度，2t/s是太慢了，但1000t/s也对本地 ...</blockquote>
有思维链的话输出还是得更高一些，毕竟思维链一般不会全看。


*****

####  lqf3dnow  
##### 58#       发表于 2025-2-1 12:39

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67324773&amp;ptid=2244823" target="_blank">宏. 发表于 2025-2-1 01:11</a>

对，这个案例实际是说CPU/GPU就不是本地运行的瓶颈，瓶颈是在满足足够存储容量之后的存储带宽，显然用显 ...</blockquote>
PCIE5.0 4x的SSD，平均带宽只有10GB/s，如果全部放在服务器多通道内存里，内存带宽有1TB左右，就算放到洋垃圾第一代志强服务器双路6通道ddr4-2666上，内存带宽也有248GB/s，这样搭配32GBx24内存，可以用不到1W元的价格攒出一台768GB内存的双路服务器，可以运行671B的全量模型。

如果优化好双路NUMA节点，达到20token的速度的速度不难，毕竟用SSD跑都有2~3token的速度


*****

####  宏.  
##### 59#         楼主| 发表于 2025-2-1 12:57

<blockquote>lqf3dnow 发表于 2025-2-1 12:39
PCIE5.0 4x的SSD，平均带宽只有10GB/s，如果全部放在服务器多通道内存里，内存带宽有1TB左右，就算放到洋 ...</blockquote>
768G不够用，跑全量R1要1362G，这是个主要限制，四路主板都不容易塞下这内存容量，但这个容量对SSD就很轻松，主板能提供128x通道的时候比较可行


*****

####  瓦格雷  
##### 60#       发表于 2025-2-1 13:06

训练和部署是两回事啊


*****

####  琉璃苑軒風  
##### 61#       发表于 2025-2-1 13:22

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67326586&amp;ptid=2244823" target="_blank">宏. 发表于 2025-2-1 12:57</a>
768G不够用，跑全量R1要1342G，这是个主要限制，单条32G四路主板都不容易塞下这内存容量，但这个容量对SS ...</blockquote>
双路霄龙24条内存配合64g单条是可以单机1536g内存

从个人角度还是很贵，但是从小公司角度也就是一张半rtx6000ada，成本低好多

—— 来自 [鹅球](https://www.pgyer.com/xfPejhuq) v3.3.96-alpha


*****

####  宏.  
##### 62#         楼主| 发表于 2025-2-1 13:31

<blockquote>琉璃苑軒風 发表于 2025-2-1 13:22
双路霄龙24条内存配合64g单条是可以单机1536g内存

从个人角度还是很贵，但是从小公司角度也就是一张半rt ...</blockquote>
对，估算了一下捡垃圾2万多元就够了，功耗不到1kw，总内存带宽能到200G，很有可能跑到10token/s


*****

####  masy  
##### 63#       发表于 2025-2-1 14:07

这配置用来训练简直灾难，跑10年能训练出现在的deepseek-r1吗？

ds导gguf进ollama，也能CPU跑推理啊，就是这输出速度挺感人。

当下的方案还是没法推翻老黄的GPU，毕竟内部还有tensor core和别的支持高速运算的核心硬件在GPU里面。


*****

####  sellboy  
##### 64#       发表于 2025-2-1 14:10

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67326984&amp;ptid=2244823" target="_blank">masy 发表于 2025-2-1 14:07</a>

这配置用来训练简直灾难，跑10年能训练出现在的deepseek-r1吗？

ds导gguf进ollama，也能CPU跑推理啊，就是 ...</blockquote>
高速总线支持多卡并联的都可以。

英特尔、AMD、老黄都有4卡、8卡的方案这些配合200多GB的HBM都足够跑原生671b了，需求极端的话老黄还有通过NVlink switch最大并72卡的用法。


*****

####  億万千  
##### 65#       发表于 2025-2-1 14:12

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67326787&amp;ptid=2244823" target="_blank">宏. 发表于 2025-2-1 13:31</a>

对，估算了一下捡垃圾2万多元就够了，功耗不到1kw，总内存带宽能到200G，很有可能跑到10token/s ...</blockquote>
个人家用两万块正常主机配置的显卡跑不到10tps吗


*****

####  orecheng  
##### 66#       发表于 2025-2-1 14:21

我觉得最大的影响是，AMD, Intel 不用去开发自家的类似cuda的生态了，把省下的钱无脑堆显存就能颠覆Nvidia了，比如1T显存的显卡卖1万USD

*****

####  宵待草  
##### 67#       发表于 2025-2-1 14:22

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67325800&amp;ptid=2244823" target="_blank">ななひら 发表于 2025-2-1 10:58</a>

感觉大家都忽略了一个问题，除了参数本身要占内存，加大上下文长度也要占很多内存。2k的上下文干不了什么活 ...</blockquote>
MLA 用的内存倒是真的不多，每个 token 大概也就 576*2*60*sizeof(dtype)。

不过 2t/s 应该是按照短上下文来算的，计算成本会随上下文长短线性增长，存得下也算不过来

*****

####  dulun59  
##### 68#       发表于 2025-2-1 14:22

想要跑得快 跑得好 目前还是得用黄狗的卡 并且也还是得用cuda

[论坛助手,iPhone](https://bbs.saraba1st.com/2b/forum.php?mod=viewthread&amp;tid=2029836)

*****

####  qratosones1337  
##### 69#       发表于 2025-2-1 14:25

华为云公众号发了，硅基流动上架了昇腾推理的R1和V3

—— 来自 [鹅球](https://www.pgyer.com/GcUxKd4w) v3.3.96


*****

####  宏.  
##### 70#         楼主| 发表于 2025-2-1 14:27

<blockquote>億万千 发表于 2025-2-1 14:12
个人家用两万块正常主机配置的显卡跑不到10tps吗</blockquote>
你两万块钱配出来的机器显存根本塞不进去全量模型

*****

####  宏.  
##### 71#         楼主| 发表于 2025-2-1 14:29

<blockquote>masy 发表于 2025-2-1 14:07
这配置用来训练简直灾难，跑10年能训练出现在的deepseek-r1吗？

ds导gguf进ollama，也能CPU跑推理啊，就是 ...</blockquote>
为什么要训练，你以为老黄卖的是训练，其实老黄卖的是钻石显存跑推理，直接用白菜内存推理不用钻石显存了老黄能不打折吗


*****

####  gammatau  
##### 72#       发表于 2025-2-1 14:40

Unified Memory还真是对的！


*****

####  x.cat  
##### 73#       发表于 2025-2-1 14:42

<img src="https://static.saraba1st.com/image/smiley/face2017/067.png" referrerpolicy="no-referrer">那内存是不是该涨价了


*****

####  treexper  
##### 74#       发表于 2025-2-1 17:35

整个深度学习领域都可以不需要gpu，是不是吓一跳？

回忆一下gpu之前的名字，加速卡。


*****

####  zmj1316  
##### 75#       发表于 2025-2-1 18:26

有没有人拿傲腾试试，毕竟随机性能无敌

—— 来自 [鹅球](https://www.pgyer.com/GcUxKd4w) v3.3.96


*****

####  btnooni  
##### 76#       发表于 2025-2-1 21:39

<img src="https://static.saraba1st.com/image/smiley/face2017/068.png" referrerpolicy="no-referrer">仔细看了下他这速度还是四通道单SSD跑出来的，提出四倍SSD也是为了抛砖引玉他自己并没有设备可以测。当然能跑2T/s跟96GB内存也有关系所以哪怕四条SSD搞raid0也不可能就变8T/s了，具体还是等人实测出结果。然后PCIe5.0 SSD貌似就没有500GB的，1T组四个还要找扩展卡价格有点冤种，但整套加起来大概也就一个4090（前提是能用。


*****

####  宏.  
##### 77#         楼主| 发表于 2025-2-1 22:11

<blockquote>zmj1316 发表于 2025-2-1 18:26
有没有人拿傲腾试试，毕竟随机性能无敌

—— 来自 鹅球 v3.3.96</blockquote>
傲腾真是死在黎明前，单条傲腾内存都做到512G了，1U能塞进去高达8T内存。就是现在捡垃圾技术难度有点高


*****

####  Sza  
##### 78#       发表于 2025-2-1 22:29

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67329677&amp;ptid=2244823" target="_blank">宏. 发表于 2025-2-1 22:11</a>

傲腾真是死在黎明前，单条傲腾内存都做到512G了，1U能塞进去高达7.5T内存。就是现在捡垃圾技术难度有点高 ...</blockquote>
我问了下deepseek“相变存储器在LLM领域的使用前景”。有趣的是它的观点中提到PCM功耗比DRAM低。
 <blockquote>相变存储器（PCM）在大语言模型（LLM）推理领域的发展前景需要结合技术特性、市场需求和竞争环境综合分析。尽管面临挑战，但在特定场景下存在潜在机会，以下是分点总结：

---

### **1. PCM的技术优势与LLM推理需求**

- **非易失性与容量潜力**  

  PCM无需持续供电即可保留数据，且存储密度高于DRAM，可能以更低成本提供更大容量，适合存储LLM的庞大参数（数百GB至TB级）。这对边缘端部署尤为重要（如本地推理设备）。

  

- **读取速度与延迟**  

  PCM的读取速度（纳秒级）虽不及DRAM，但显著快于NAND闪存，若架构优化（如缓存分层），可能缓解LLM推理时的权重加载瓶颈。

- **能耗优化**  

  相比DRAM，PCM的静态功耗更低，适合对能效敏感的部署场景（如数据中心或移动设备）。

---

### **2. 当前技术瓶颈与挑战**

- **写入速度与耐久性**  

  PCM的写入速度较慢（微秒级）且写入次数有限（约1e8次），但LLM推理以读取为主，写入需求较少（如模型更新频率低），这一弱点可能被部分规避。

- **带宽限制**  

  LLM推理需要高内存带宽以快速访问参数，PCM的带宽目前难以匹敌DRAM，需依赖架构创新（如近存计算、3D堆叠）或混合存储系统。

- **生态与产业链成熟度**  

  英特尔傲腾的停产反映了非易失性内存（NVM）商业化难度（成本、良率等）。PCM需克服类似问题，依赖头部厂商（如三星、美光）的持续投入。

---

### **3. 潜在应用场景**

- **边缘推理设备**  

  结合PCM的非易失性和容量优势，可在手机、IoT设备等边缘端部署轻量级LLM，减少对云端依赖。

- **混合存储架构**  

  与DRAM组成分层存储系统：热数据存于DRAM，冷数据存于PCM，降低整体成本同时保持性能。

- **近存计算（Near-Memory Computing）**  

  利用PCM的高密度特性，将存储与计算单元紧耦合，减少数据搬运延迟，提升推理效率。

---

### **4. 竞争技术对比**

- **MRAM/ReRAM**  

  竞品如磁性存储器（MRAM）和阻变存储器（ReRAM）在速度、耐久性上可能优于PCM，但成本更高，技术成熟度更低。

  

- **HBM与GDDR**  

  现有高带宽内存（HBM）仍是LLM硬件的首选，但成本极高，PCM若能在性价比上突破，可能成为补充方案。

---

### **5. 结论：谨慎乐观**

PCM在LLM推理中的前景取决于：

- **技术突破**：提升带宽、降低成本，并适配AI加速器架构（如与GPU/TPU协同）。

- **场景适配**：聚焦边缘计算、混合存储等差异化需求，而非直接替代DRAM。

- **行业支持**：需头部芯片厂商、云服务商共同推动生态建设。

短期内，PCM更可能作为存储体系的补充，而非核心角色；长期看，若技术成熟且成本可控，可能在特定领域（如边缘AI）占据一席之地。</blockquote>


*****

####  廿九  
##### 79#       发表于 2025-2-2 01:24

今天刚在自家3080电脑上搞了deepseek一键包，32b的模型就是2token每秒<img src="https://static.saraba1st.com/image/smiley/face2017/067.png" referrerpolicy="no-referrer">

—— 来自 [鹅球](https://www.pgyer.com/GcUxKd4w) v3.3.96


*****

####  supif  
##### 80#       发表于 2025-2-2 01:29

deepseek别的不知道，利好硬件升级是真的。


*****

####  UniqueDiablo  
##### 81#       发表于 2025-2-2 03:16

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67324641&amp;ptid=2244823" target="_blank">frankCC 发表于 2025-2-1 00:41</a>
你看下帖子内容啊，每秒 2token 的输出黄花菜都凉了，这帖子纯粹为了迎合反老黄的情绪，一点实用性都没有。 ...</blockquote>
前几年确实有挖硬盘的


*****

####  harry3  
##### 82#       发表于 2025-2-2 11:27

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67331101&amp;ptid=2244823" target="_blank">UniqueDiablo 发表于 2025-2-2 03:16</a>

前几年确实有挖硬盘的</blockquote>
硬盘币是硬盘币，和AI没一点关系啊，本来就是搞p2p那群人设计的

