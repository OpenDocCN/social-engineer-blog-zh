# 通过社会工程窃取凭证

> 原文：<https://www.social-engineer.org/social-engineering/stealing-credentials-via-social-engineering/>

Social-Engineer.org 收到了许多对社会工程感兴趣的人提交的材料，这些社会工程包括社会工程、T2、欺骗、身份盗窃、信息收集以及其他真正的社会工程师。最近，一个 social-engineer.org 的粉丝，卡什，写了一篇非常有趣的关于窃取证书的文章/故事。我们希望您能像我们一样喜欢它，并请继续将您的[提交给我们](/cdn-cgi/l/email-protection#44272b2a30362d2631302104372b272d252869212a232d2a2121366a2b3623)。

**背景**

几年前，我为一个客户进行了一次社会工程实践，目标是找出公司运营程序中可能存在的缺陷，这些缺陷可能会允许某人破坏员工的企业 Web 访问(EWA)凭据、单一用户 id 和密码，从而允许访问多个内部系统。

主要目的是破坏某人的现有密码，这将提供持续的机会，以秘密模式访问各种公司系统。

这个练习展示了攻击者(潜在的内部威胁)通过非技术手段，主要是通过[电话](https://www.social-engineer.org/framework/general-discussion/common-attacks/phone/)，在很短的时间内可以完成的[。](https://www.social-engineer.org/framework/general-discussion/typical-goals/)

**最终目标**

我的最终目标是通过基本的社会工程策略从该公司的帮助台员工那里提取信息，以进一步利用该组织的企业 Web 访问(EWA)系统中的一些已知问题。特别是，我想利用以下缺陷:

更改 EWA 密码不需要输入旧密码。这意味着，经过身份验证的用户可以在不提供旧密码的情况下将帐户密码更改为新密码。因此，潜在地，有机会手动更改某人的密码，而不知道原来的密码。一旦通过验证，现有机密问题的答案将以明文形式呈现。一旦受到威胁，帐户可能总是通过原始的机密问题和答案受到威胁。
当密码或机密问题被修改时，不会向用户发送电子邮件通知来告知此类更改，从而允许用户恢复并重置密码。该缺陷将允许攻击者通过更改机密问题并阻止用户恢复其受损帐户来完全拥有受损帐户。

EWA 应用程序中的这些漏洞非常严重，因为无人值守的浏览器会话很容易受到攻击，其密码也很容易被更改。在这种情况下，机密问题与密码一样重要，因为它们允许用户重置密码，并充当另一种形式的身份验证。

鉴于上述一些应用程序漏洞，特别是最后两个，我的目标是确定我是否可以利用帮助台来帮助我解决以下任何问题，同时只提供有限的个人或其他身份信息:

帮我重置目标的机密问题和答案
帮我找回目标现有机密问题的答案
只需通过电话告诉我密码

**一般信息收集阶段**

像任何社会工程练习一样，在[侦察和准备](https://www.social-engineer.org/framework/information-gathering/physical-methods-of-information-gathering/)中花费了大量的时间来学习公司的行话、各部门的电话号码和基本的操作程序。这一过程的明确目标是收集尽可能多的[相关信息](https://www.social-engineer.org/newsletter/Social-Engineer.Org%20Newsletter%20Vol.%2004%20Iss.%2043.htm)。

**攻击阶段**

**第一步**

有针对性的[信息收集阶段](https://www.social-engineer.org/framework/information-gathering/)确定潜在的好目标:这一阶段的目标是找到一个合法的目标和一些关于他的基本可识别信息。

*注意*:一名新员工通常会给社会工程师带来最好的机会。一个新员工往往胆小怕事，不熟悉内部流程，他们总想给别人留下深刻印象，从来不难看。

*步 1A:* [叫露西](https://www.social-engineer.org/framework/general-discussion/common-attacks/phone/)公司培训部的接待员:

“你好，Lucy，我是 IT Web Group 的执行产品经理 Emile Woodson。你们最近为我们促成了一次出色的培训，我想给你们的运营经理写封感谢信。我写给谁？”

“哦那太好了。你可以寄给杰克·马尔泰伯。”

“太好了。我不知道杰克还在管理那个组织。我也应该在今天会议结束后给他打个电话。能不能请你提醒我他的分机号码，并告诉我他是否会在下午 5 点左右？”

“当然，他的分机号码是 xxx-8844，他到这里很早，通常在 4:30 左右离开；所以你可能想早点给他打电话。”

我不想在检索到我想要的数据后就结束对话。因此，在挂断电话之前，我就他们的培训服务进行了一些随意和普通的交谈。

*注意:* Lucy 提供了这些信息，因为她认为这些信息并不敏感，尤其是因为她将这些信息提供给了一位同事，一位心怀感激的执行产品经理！

*步骤 1B:* [假冒我的来电显示](https://www.social-engineer.org/framework/se-tools/phone/caller-id-spoofing/)显示杰克的号码，xxx-8844，下午 5 点打电话给人力资源部。

“嗨，我是杰克·马尔泰伯，公司培训部的高级运营经理。我打电话是因为我们正在对所有新员工进行年度强制合规培训，我们需要从您那里得到这份清单。我们需要过去 6 个月所有新员工的名单。请确保包括雇佣日期及其 EUIDs(员工用户 ID)。我们的首席合规官 Gina Blackstone 指示我们明天通过 COB 向所有学员发送电子邮件。如果您能尽快将该信息发送给我的首席分析师，我将不胜感激”

“当然可以。我可以在一小时内通过电子邮件发送信息。”

"事实上，如果你能传真给她就太好了."

"没问题，她的名字和传真号码是什么？"

*注:*紧迫性和[权威](https://www.social-engineer.org/framework/influencing-others/influence-tactics/authority/)是这里的关键要素。一个标准的社会工程策略被用来产生一个有组织的混乱。利用一种想顺从一个“权威人物”的人类情感。同样，她在帮助公司内部的某个人，她认为这些信息无关紧要。

我从名单中找到了一个潜在的好目标，何塞·维罗，市场部的新员工。

**第二步**

[冒充](https://www.social-engineer.org/framework/general-discussion/common-attacks/tech-support/)目标并呼叫帮助台:这部分练习首先使用一部电话和一个来电显示欺骗器通过电话联系帮助台以启动密码重置。帮助台代表通过询问我的姓名和我的员工用户 ID (EUID)接了电话。一旦我提供了目标的名字和 EUID，我告诉他我需要 EWA 系统的帮助。我告诉他我忘记了我的秘密问题的答案，以及他是否可以通过电话提供给我。答案是“不，我们无法获得这些信息”。然后我问他能否通过电话更改我的秘密问题，这样我以后就可以重新设置自己的密码。同样，答案是“不，我们没有这个能力”。

然后，我说我无法立即访问我的公司电子邮件来接收我的新密码重置链接，并询问是否有办法通过电话获取新密码。支持代表提到，通过电话重置和提供临时密码是常规做法。我找到进去的路了！然后他告诉我我的名、中名、姓，问对不对。我说“是”。然后他问我是否在 23 号楼工作。我答应了！然后他要了我的社会安全号码的后四位数字。

啊哦！我还没准备好，所以必须尽快想出办法。

"通过电话提供我的社会安全号码让我感到不舒服."

“嗯，先生，我们只需要最后 4 位数字，这是通过电话重置您的密码的唯一方法。”

“我明白。让我考虑一下。也许我可以再试一次我的秘密问题。我只是不喜欢在电话里提供任何敏感信息。因为我是新来的，我需要向我的主管确认一下。我会保持联系的。”

**第三步**

泄露目标 SSN 的最后四位数字:在这部分练习中，我想探究[所有可能导致泄露目标社会安全号码最后四位数字的攻击媒介](https://www.social-engineer.org/framework/attack-vectors/)。这些信息可以通过标准的社交
工程策略获得，也可以通过暴力破解几个不提供账户锁定的内部应用程序之一获得。

*步骤 3A:技术方法*

员工 ID Lookup 是一个内部 web 应用程序，它为所有员工提供了一个查找员工 ID 的自助服务解决方案。经过一些检查，很明显，应用程序没有实现任何类型的查找锁定。所以本质上，任何字段都可能受到暴力攻击。在应用了名字和姓氏之后，我可以列举有效的 SSN 信息。这是一个简单的暴力攻击，会泄露任何雇员的 SSN 的最后四位数字。更具体地说，我使用了 Burp Suite Intruder，这是一个很好的工具，可以针对这种情况自动进行定制的暴力攻击。

![ Stealing Credentials via Social Engineering](img/019fe0d6967592845628ab5e107fb7f1.png)
图 1–SSN 的后四位数字可以通过提供该人的名和姓来检索。如果 SSN 的最后 4 位数字是正确的，将检索一个员工 ID；否则，将显示一条错误消息

*迈步 3B:低技术方法*

用预付费电话给受害人 Jose Vero 打了个电话，并伪造了来电显示。

“你好荷西。我是公司旅游部的李尚义。我拿到了你去新奥尔良参加营销会议的机票，我想知道你是去取，还是用办公室间邮件寄给你？”

“我想我没有去新奥尔良旅行的计划。这一定是个错误。”

“嗯，何塞，有人为你提出了一个请求，我们现在有你的票。让我核实一下你的名字。你的全名是何塞·韦罗吗？”

“是的。”

“在市场部？”

“是的。”

“让我再做一次查找，看看是谁为您提出了这个请求。您的社会保险号的后 4 位数字是多少？”

“8895.”

“谢谢你何塞。”

真的谢谢你！

**第四步**

重置密码。

掌握了所有信息后，我再次打电话给帮助台，重新设置 Jose Vero 的企业 Web 访问密码。该代表要求提供所有必需的信息，包括社会保险号的最后四位数字，我提供了这些信息，并收到了一个临时密码“temppwd123”。

使用这些信息，我可以通过验证和查看机密问题的答案来完全拥有该帐户。

耗时 60 分钟。游戏结束。

如前所述，由于应用程序漏洞，Jose Vero 从未收到电子邮件通知来了解他的密码被更改。他只是认为他忘记了密码，这是常有的事。几天后，他使用“有缺陷的”密码重置方案和机密问题重新获得访问权限，并继续使用该帐户，没有任何怀疑。Jose 不知道我已经进入了他的帐户，查看了他的秘密问题的答案，因为提到的应用程序漏洞之一，我总是可以使用相同的秘密问题和答案返回。

**结论**

想要信任他人、[让他人开心](https://www.social-engineer.org/framework/influencing-others/influence-tactics/liking/)以及顺从同事和组织中的其他权威人物是人的天性。从这个练习以及其他类似的练习中可以得出的相关结论是，每个人都容易受到社会工程攻击。不管是时间不够，还是身体疲劳，都有我们走精神捷径，没有把每件事都处理细致的时候；这就是我们脆弱的时候。

遏制或防止社会工程攻击的最佳方式是培训您的员工。训练他们在日常交往中保持一定程度的谨慎。训练他们了解他们不能对这类攻击免疫，并向他们展示如何检测和保护自己免受这类攻击。不断提醒你的员工，所有的信息，无论他们认为多么琐碎和无关紧要，都可能帮助一个社会工程师得到他想要的东西。

(由 [Khash Kiani](https://www.social-engineer.org/blog/aboutus/) 捐赠给 social-engineer.org)

关于这个话题的更多信息，请查看我们关于身份盗窃的[播客](https://www.social-engineer.org/podcast/episode-008-the-social-engineering-zero-day-revealed/)