
*****

####  kanzakiken  
##### 1#       楼主       发表于 2025-2-19 11:36

用的是deepseek-R1的模型，昨天提问了几个问题，每次提问都不到20个字，但是输入tokens就已经消耗了快10w了，输出tokens消耗了1.6w，感觉还算正常。

检查了一下我chatbox设置的上下文的消息数量上限是20，难道是上下文消息太多，导致未命中缓存的token太多，从而导致输入tokens变多吗？

*****

####  overflowal  
##### 2#       发表于 2025-2-19 11:40

<img src="https://static.saraba1st.com/image/smiley/face2017/048.png" referrerpolicy="no-referrer">对话的原理就是把你的前面所有内容再塞回LLM里，然后下一次输出。不是每次只塞你的输入。它的输出也会塞回去

*****

####  med  
##### 3#       发表于 2025-2-19 11:46

没这功能llm会失忆的<img src="https://static.saraba1st.com/image/smiley/face2017/067.png" referrerpolicy="no-referrer">

*****

####  神剑烧鸡  
##### 4#       发表于 2025-2-19 11:48

<img src="https://static.saraba1st.com/image/smiley/face2017/067.png" referrerpolicy="no-referrer">你猜为什么输入token的计费比输出低很多

*****

####  爱莉希雅  
##### 5#       发表于 2025-2-19 11:51

每次的问题不相关的话需要清空上下文关联或者新开个对话

*****

####  StrangerJ  
##### 6#       发表于 2025-2-19 11:52

原来如此，看了下统计2天用了20万token<img src="https://static.saraba1st.com/image/smiley/face2017/103.png" referrerpolicy="no-referrer">

*****

####  原装大小姐  
##### 7#       发表于 2025-2-19 12:02

你用chatbox看看不就知道了，平均一次约10000

—— 来自 [鹅球](https://www.pgyer.com/xfPejhuq) v3.3.96-alpha

*****

####  Nanachi  
##### 8#       发表于 2025-2-19 12:03

think的内容也算token

—— 来自 [鹅球](https://www.pgyer.com/GcUxKd4w) v3.3.96

*****

####  bixinhaner  
##### 9#       发表于 2025-2-19 12:30

可以设定几轮对话历史吧。设置5轮以内就差不多了

*****

####  流缨  
##### 10#       发表于 2025-2-19 14:10

如果你是用他家BOT也就是加联网那个调法会更多更多的，因为RAG塞进去的也算输入，且100%不能命中缓存

*****

####  嘎嘣脆  
##### 11#       发表于 2025-2-19 14:29

昨天问了strawberry有几个r，丫颠来倒去反复思考

就是这么刷计件工资的吗<img src="https://static.saraba1st.com/image/smiley/face2017/053.png" referrerpolicy="no-referrer">

*****

####  云在青天  
##### 12#       发表于 2025-2-19 14:58

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67465531&amp;ptid=2246730" target="_blank">嘎嘣脆 发表于 2025-2-19 14:29</a>

昨天问了strawberry有几个r，丫颠来倒去反复思考

就是这么刷计件工资的吗</blockquote>
思考也算吗，好家伙

*****

####  harukage  
##### 13#       发表于 2025-2-19 15:02

我用的是硅基流动的api。让deepseek帮我改代码，主程序直接往里面丢，一天也就十万token

—— 来自 [鹅球](https://www.pgyer.com/GcUxKd4w) v3.3.96

*****

####  秦南心  
##### 14#       发表于 2025-2-19 15:07

提示: 作者被禁止或删除 内容自动屏蔽

*****

####  luodang007  
##### 15#       发表于 2025-2-21 18:38

大佬们有邀请码吗？好像用邀请码注册有券领，能发我一个吗，谢谢<img src="https://static.saraba1st.com/image/smiley/face2017/072.png" referrerpolicy="no-referrer">

*****

####  2sunur  
##### 16#       发表于 2025-2-21 18:45

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67487676&amp;ptid=2246730" target="_blank">luodang007 发表于 2025-2-21 18:38</a>

大佬们有邀请码吗？好像用邀请码注册有券领，能发我一个吗，谢谢</blockquote>
[https://www.volcengine.com/exper ... QY5&amp;rc=Y51MUBS5](https://www.volcengine.com/experience/ark?utm_term=202502dsinvite&amp;ac=DSASUQY5&amp;rc=Y51MUBS5)

谢谢谢谢<img src="https://static.saraba1st.com/image/smiley/face2017/044.png" referrerpolicy="no-referrer">

*****

####  sellboy  
##### 17#       发表于 2025-2-21 18:50

火山好像没有输入缓存命中情况单独计费。

连续对话的上文很大比例是会缓存命中的，如果分别计费能便宜很多。

*****

####  2sunur  
##### 18#       发表于 2025-2-21 19:02

目前几家主流提供deepseek的api平台我用下来看，火山和秘塔似乎是比较快的，硅基流动的pro有时候都磨磨唧唧的

*****

####  jeokeo  
##### 19#       发表于 2025-2-21 22:30

顺便问问

chatbox里面把上下文设置无限，但是似乎还是有限的，这个极限是多少？r1

*****

####  有鱼  
##### 20#       发表于 2025-2-21 22:45

我感觉r1的消耗量都还行，拿火山的dsv3来翻译大量文本的token消耗真的有点贵

*****

####  thq  
##### 21#       发表于 2025-2-22 13:01

火山的计算和别家应该不一样， 同样用cline， 我用火山的最多三个来回就消耗了50万欠费，而换成派欧算力云的，五十万个token用了三四天

*****

####  阿斯蓝  
##### 22#       发表于 2025-2-22 14:09

火山引擎邀请链接，可以一起薅一点代金券

https://www.volcengine.com/experience/ark?utm_term=202502dsinvite&amp;ac=DSASUQY5&amp;rc=CX7DMWHW

*****

####  harry3  
##### 23#       发表于 2025-2-22 14:16

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67492052&amp;ptid=2246730" target="_blank">thq 发表于 2025-2-22 13:01</a>

火山的计算和别家应该不一样， 同样用cline， 我用火山的最多三个来回就消耗了50万欠费，而换成派欧算力云 ...</blockquote>
确实，火山的50w我也是一两天就用完了，欧派云的50w到现在一周多了才用了一半

*****

####  革萌  
##### 24#       发表于 2025-2-22 14:17

<img src="https://static.saraba1st.com/image/smiley/face2017/022.png" referrerpolicy="no-referrer">Deepseek官网最好的一点就是命中cache打骨折

现在第三方的apii好像都没有这个机制

*****

####  sjax001  
##### 25#       发表于 2025-2-22 14:50

 本帖最后由 sjax001 于 2025-2-22 14:52 编辑 

派欧云有邀请码吗求一个！

*****

####  天知道  
##### 26#       发表于 2025-2-22 15:11

我用的硅基的，真的很耗：16元100万，基本上我每次对话至少5000，多的10000也有。算起来就是一次8分到1毛6

*****

####  chaoswing  
##### 27#       发表于 2025-2-22 15:16

火山我打开了知识库，上传了5个文件，不到200页吧，一天扣了我十几块<img src="https://static.saraba1st.com/image/smiley/face2017/068.png" referrerpolicy="no-referrer">

*****

####  无名小卒  
##### 28#       发表于 2025-2-22 15:45

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67492820&amp;ptid=2246730" target="_blank">chaoswing 发表于 2025-2-22 15:16</a>
火山我打开了知识库，上传了5个文件，不到200页吧，一天扣了我十几块</blockquote>
知识库开了，就算什么都没有，一小时四毛五<img src="https://static.saraba1st.com/image/smiley/face2017/068.png" referrerpolicy="no-referrer">好像

—— 来自 [鹅球](https://www.pgyer.com/GcUxKd4w) v3.3.96

*****

####  zerona  
##### 29#       发表于 2025-2-22 16:05

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67492943&amp;ptid=2246730" target="_blank">无名小卒 发表于 2025-2-22 15:45</a>

知识库开了，就算什么都没有，一小时四毛五好像

—— 来自 鹅球 v3.3.96</blockquote>
不操作都有消耗？

*****

####  无名小卒  
##### 30#       发表于 2025-2-22 16:09

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67493045&amp;ptid=2246730" target="_blank">zerona 发表于 2025-2-22 16:05</a>
不操作都有消耗？</blockquote>
知识库相当于云服务器吧，开了就相当于开着一台电脑，按小时收费，上传文件另外计费。

—— 来自 [鹅球](https://www.pgyer.com/GcUxKd4w) v3.3.96

*****

####  zerona  
##### 31#       发表于 2025-2-22 16:11

 本帖最后由 zerona 于 2025-2-22 17:32 编辑 
<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67493063&amp;ptid=2246730" target="_blank">无名小卒 发表于 2025-2-22 16:09</a>

知识库相当于云服务器吧，开了就相当于开着一台电脑，按小时收费，上传文件另外计费。

—— 来自 鹅球 v ...</blockquote>
那page assist 的知识库呢？

我试着传了个文件，看用的嵌入模型是我之前下的deepseek r1。 这个就可以用自己的知识库了吧？

褥个羊毛
[https://www.volcengine.com/exper ... QY5&amp;rc=TMIIPZY2](https://www.volcengine.com/experience/ark?utm_term=202502dsinvite&amp;ac=DSASUQY5&amp;rc=TMIIPZY2)

*****

####  mortal1976  
##### 32#       发表于 2025-2-22 16:37

<blockquote>无名小卒 发表于 2025-2-22 15:45
知识库开了，就算什么都没有，一小时四毛五好像

—— 来自 鹅球 v3.3.96</blockquote>
为何不用coze平台呢？就算国外版上不了，国内版也有r1和qwen max可以免费用，知识库也是**的。

*****

####  御坂MKII  
##### 33#       发表于 2025-2-22 16:57

之前看文档，火山的缓存是需要用 api 具体的创建一个 session 的，裸用可能是没有缓存的

—— 来自 [鹅球](https://www.pgyer.com/GcUxKd4w) v3.3.96

*****

####  嗜酸性粒细胞  
##### 34#       发表于 2025-2-22 17:11

火山引擎的邀请码，可以薅点羊毛
[https://www.volcengine.com/exper ... QY5&amp;rc=KWRL179F](https://www.volcengine.com/experience/ark?utm_term=202502dsinvite&amp;ac=DSASUQY5&amp;rc=KWRL179F)

*****

####  chaoswing  
##### 35#       发表于 2025-2-22 17:48

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67493045&amp;ptid=2246730" target="_blank">zerona 发表于 2025-2-22 16:05</a>
不操作都有消耗？</blockquote>
楼上说的很对，我也是四毛五一个小时
他这个付费比较复杂，有向量化的计算费用，有根据存储量和存储时间的费用
我估计是只要你建立了知识库，光那个索引就是最低四毛五

所以还是用rag吧

*****

####  chaoswing  
##### 36#       发表于 2025-2-22 17:49

我意思是本地rag，不要用火山提供的

*****

####  バーチャルS1er  
##### 37#       发表于 2025-2-22 17:54

官网试着写小说。越写到后面**时间就越长，还会发生字数减少，一个问题页面还是不要问太多次好

*****

####  shqingda_  
##### 38#       发表于 2025-2-24 18:45

火山引擎邀请链接，有羊毛一起薅<img src="https://static.saraba1st.com/image/smiley/face2017/033.png" referrerpolicy="no-referrer">

*****

####  gabriel233  
##### 39#       发表于 2025-2-26 13:38

DeepSeek满血版免费领啦！邀请好友注册和使用，最高双方可获得145元代金券，免费抵扣3625万tokens，畅享R1与V3模型！参与入口：[https://www.volcengine.com/exper ... QY5&amp;rc=OLB5ECEW](https://www.volcengine.com/experience/ark?utm_term=202502dsinvite&amp;ac=DSASUQY5&amp;rc=OLB5ECEW)  邀请码：OLB5ECEW

*****

####  char1st  
##### 40#       发表于 2025-2-26 14:02

要不楼上几个建个aff专楼吧。


*****

####  Luck  
##### 41#       发表于 2025-3-17 14:29

类似的问题，我是用cherrystudio建了本地知识库，用火山API接了DS R1，今天发现我5号消耗了12W token（几乎全部是输入），然而我5号只问了2个问题，怀疑是提交prompt的时候把知识库检索出来的相关内容一并提交了，按照这个节奏，知识库越大提问越消耗token，不知道如何解决…………<img src="https://static.saraba1st.com/image/smiley/face2017/001.png" referrerpolicy="no-referrer">


*****

####  overflowal  
##### 42#       发表于 2025-3-17 14:32

现在你们知道deepseek官方的无感默认cache有多仁慈了吧<img src="https://static.saraba1st.com/image/smiley/face2017/037.png" referrerpolicy="no-referrer">

—— 来自 [鹅球](https://www.pgyer.com/GcUxKd4w) v3.3.96


*****

####  望上弦  
##### 43#       发表于 2025-3-19 14:15

我靠，怪不得我才几天就把免费额度干完了，我基本都只在一个聊天框里问问题<img src="https://static.saraba1st.com/image/smiley/face2017/004.gif" referrerpolicy="no-referrer">

—— 来自 vivo V2199A, Android 14上的 [S1Next-鹅版](https://github.com/ykrank/S1-Next/releases) v2.5.4


*****

####  Elicasa  
##### 44#       发表于 2025-3-19 14:25

<blockquote>引用第40楼Luck于2025-03-17 14:29发表的  :

类似的问题，我是用cherrystudio建了本地知识库，用火山API接了DS R1，今天发现我5号......</blockquote>
没法解决，大语言模型就是这个玩法，不把检索出的知识库内容一起输入，又如何让模型知道信息来给出回答呢？

----发送自 [Sony XQ-AT72,Android 12](http://stage1.5j4m.com/?1.42)


*****

####  约翰里德  
##### 45#       发表于 2025-3-19 14:30

我一个跑团回答33000tokens，我抱怨了吗<img src="https://static.saraba1st.com/image/smiley/face2017/067.png" referrerpolicy="no-referrer">


*****

####  moekyo  
##### 46#       发表于 2025-3-19 14:32

本地部署可破<img src="https://static.saraba1st.com/image/smiley/face2017/067.png" referrerpolicy="no-referrer">

<img src="https://img.saraba1st.com/forum/202503/19/143138tq0w2ozzocpd0ac2.png" referrerpolicy="no-referrer">

<strong>image.png</strong> (74.68 KB, 下载次数: 0)

下载附件

2025-3-19 14:31 上传

[https://huggingface.co/bartowski ... -Instruct-2503-GGUF](https://huggingface.co/bartowski/mistralai_Mistral-Small-3.1-24B-Instruct-2503-GGUF)


*****

####  zy450  
##### 47#       发表于 2025-3-19 15:27

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67686237&amp;ptid=2246730" target="_blank">moekyo 发表于 2025-3-19 14:32</a>

本地部署可破

https://huggingface.co/bartowski/mistralai_Mistral-Small-3.1-24B-Instruct-2503-GGUF ...</blockquote>
这是之前说的欧洲AI？不是说欧洲上不了桌吗


*****

####  moekyo  
##### 48#       发表于 2025-3-19 15:35

<blockquote><a href="httphttps://bbs.saraba1st.com/2b/forum.php?mod=redirect&amp;goto=findpost&amp;pid=67686587&amp;ptid=2246730" target="_blank">zy450 发表于 2025-3-19 15:27</a>

这是之前说的欧洲AI？不是说欧洲上不了桌吗</blockquote>
怎么讲呢，创始人是 Deepmind 和 Meta 的前员工，看你定义了，不过肯定比纯血法国的 Lucie 好多了<img src="https://static.saraba1st.com/image/smiley/face2017/044.png" referrerpolicy="no-referrer"> 


*****

####  kouym  
##### 49#       发表于 2025-3-19 15:42

所以每问一个新的问题 跟前面无关的 新增一个会话最好 不是的话会把之前上下文全带进去


*****

####  CrayS1  
##### 50#       发表于 2025-3-19 16:18

看openai底层库就知道 ，每次提问的时候会把所有的历史聊天记录都重新发一遍。


*****

####  ななひら  
##### 51#       发表于 2025-3-19 16:21

无所谓啦，这才几个钱<img src="https://static.saraba1st.com/image/smiley/face2017/067.png" referrerpolicy="no-referrer">

