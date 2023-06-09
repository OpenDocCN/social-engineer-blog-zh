# 社交媒体工程的节拍

> 原文：<https://www.social-engineer.org/social-engineering/the-beat-of-social-media-engineering/>

最近，罗格斯大学发表了一篇关于 API 工具“The Beat”的文章，这似乎是社交媒体信息更有趣的用途之一。Beat 将 Instagram 图片中嵌入的地理信息链接到谷歌街景。然后，使用 Instagram 上的标签就可以搜索到这些内容。API 和信息收集在 [社交工程师播客 039](https://www.social-engineer.org/podcast/episode-039_information_gathering_on_steroids/ "SEPodcast #39") 中有所涉及。

从表面上看，它似乎是一个神奇的工具。用户可以搜索他们参加的音乐会的标签，找到其他也在那里的人，并查看他们的照片——因为社交工程师播客并不真正关注“如何免费找到女孩”，这可能是“The Beat！”

然而，当我们在办公室讨论这个工具的安全含义时，我们决定搜索更多不寻常的项目。当我们发现，搜索更多的通用术语，我们发现了 API 的阴暗面。

通过搜索日光浴,“The Beat”会显示带有日光浴标签的图片。这最初带来了猫和狗的主人拍摄的日光浴——都与一个大致的地址相关联。当猫的图像经过时，一个人晒日光浴的相当淫秽的图像出现了。他们把照片从她的身体一直带到他们的脚下。照片包括描述和标签:

**Instagram 挑战赛第 7 天——妈妈的花园如此美丽# insta gram challenge # insta gram daily # insta picture # insta gram #五彩缤纷#挑战赛#植物#粉色#花朵#花朵#日光浴#晒黑#夏天#阳光充足#太阳#花园#绿色#妈妈#自然#楼梯#色彩**

用户参加了 Instagram 挑战，用某些关键词拍照。

用户还使用他们的全名(包括中间名)作为他们的 Instagram 用户名，例如 **John P. Smith**

关键是“The Beat”还提供了完整的邮政地址，包括谷歌街景提供的门牌号。

通过在谷歌中搜索用户的姓名和地址，他们的父亲的详细信息被披露出来，因为他在家经营一家电气企业。这给了我们他的邮政地址、电话号码和手机号码。

作为 Instagram 个人资料的一部分，用户还包括:

*   BBM 数
*   Kik 配置文件名称
*   Tumblr 账户

此时，在两个网页和一次网络搜索中，我们找到了全名、地址、电话号码、手机品牌和型号以及照片。

作为研究的一部分，我们决定继续搜索，看看我们能找到多少关于这个随机用户的信息。在进入“关于我”页面之前，进入该用户 Tumblr 账户的个人资料不会显示任何直接信息。这便也摆摆手:

*   Twitter 句柄
*   出生日期
*   位置
*   高度
*   喜欢
*   BBM 销(再次)
*   脸书·佩奇
*   关系状态

通过从这里搜索到用户的脸书页面，我们确认了他们的出生日期，然后确定了父母的详细信息，兄弟姐妹(他们也曾和父亲一起工作)。

Twitter 还交出了他们的社团和所在地(包括大学)的名单。

**Exploit Used** :用户对社交网络的信任，而没有考虑恶意用户会如何使用他们的信息来定位他们。

**漏洞暴露**:社交媒体泄露太多信息，对社交媒体的信任，用户缺乏安全意识。

**补丁**:

1)永远不要把这么多信息放到网上

2)对网络安全风险的教育不够

3)在网上把这些点联系起来很容易

4)一份完整的身份资料需要 10 分钟，因为有人对自己的信息如此开放

5)社会工程师无需深究贴出的文字，就能从图片中获得有价值的信息！

6)关闭你的位置

7)不要使用你的用户名…哦，等等，那是我的名字！

让我们不要像打算使用这个工具的消费者那样思考，而是像恶意用户或社会工程师那样思考。你会进行什么样的搜索？

*   借记卡
*   信用卡
*   办公室
*   部门
*   酷派办公
*   工作
*   保安摄像机
*   书桌
*   安全性
*   停车场
*   肥皂，肥皂

*   <road name=""></road>
*   <target company="" name=""></target>

现在我们开始了解黑客的心理。我们开始考虑社交媒体类型、有多少数据被共享，以及数据从他们的办公桌、办公室、区域、环境中暴露的可能性，这些都可能与用户的位置相关联。

自从 Rutgers 系统的最初发布以来，运营商已经概括了显示的地址，仅显示道路名称和区域，而不是实际的地址号码。然而，这不足以隐藏这些信息，因为使用谷歌街景可以很容易地从照片中猜出地址。

通过搜索公司名称或相关细节，你可以很容易地找到办公室(里里外外)的照片，可能还有制服、身份证和社交习惯。所有这些对于信息收集部分甚至是启发都是至关重要的，

随着更多的信息被添加到社交媒体平台(“大数据”)，更多的信息可以被利用。我们的预测是，随着 API 变得更加开放，我们将看到更多的服务推出，因此互联网将成为那些想要发起社会工程师攻击的人的更大的游乐场。

由 Secarma 的 Stuart Coulson 撰写的客座博文

**关于塞卡尔玛**

Secarma 最初是云和网络托管提供商 UKFast 的内部部门，于 2012 年 9 月开始作为一家独立公司运营，专注于灾难恢复服务和业务连续性。凭借为许多不同行业提供危机管理和道德安全测试的令人印象深刻的记录，BBC 屡获殊荣的广播节目《裸体科学家》(The Naked Scientists)利用 Secarma 的专业知识来调查数据安全——在易贝购买格式化硬盘，并将其发送到 Secarma，目的是恢复数据。塞卡尔马随后被邀请讨论他们的调查结果，作为第五电台直播节目“科学之夜”的一部分。