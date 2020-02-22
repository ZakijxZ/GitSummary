# 软件版本周期

![Software_dev2](VersionSuffixAndCodeReview.assets/Software_dev2.svg)

## Testing&Dev开发期

- Pre-alpha:是alpha前的是一个功能不完整的版本，开发最初。

- α（Alpha）版:内测版，一般开发者及组织内部使用，Bug较多。

- β（Beta）版:公测版，公众大规模测试用，存在一些缺陷。

- RC（Release Candidate）版:发布候选版本，这阶段亦称λ(Gamma)阶段（更后期的称为[Delta](https://baike.baidu.com/item/Delta/15417786)，及其后的希腊字母），该版本已经完成全部功能并清除大部分的BUG。从Alpha到Beta再到Gamma是改进的先后关系，但RC1、RC2往往是取舍关系。

  注:aka是also known as,广为人知

- SR版:Service Release的缩写,修正版或更新版,修正了正式版推出后发现的Bug

- Final:正式版

## Release完成期

- Release版:发行版, 在前面版本的一系列测试版之后，得到交付用户使用的正式版本，一般为标准版。一般情况下，Release不会以单词形式出现在软件封面上，取而代之的是符号®。
- RTM（Release to Manufacting）:生产商发放,软件产品准备交付生产商时使用。
- RTW（Release to Web）:网络分发,一种利用互联网进行分发的软件交付客户的方式。
- Stable:稳定版，来自预览版本释出使用与改善而修正完成。
- RTL(Retail):零售版，是真正的正式版，正式上架零售版。
- GA(General Availability):一般可用，所有必要的商业活动已经完成，官方开始推荐广泛使用，进入发售的阶段。在国外都是用GA来说明**release版本**的
- OEM(Original Equipment Manufacturer)版:厂商定制版,只能随计算机一起贩卖;只能重新安装，不能升级产生。包装不像零售版精美，通常只有一面CD和说明书(授权书)。
- EVAL版:评估版,有30或者60天等使用期限。
- RVL:它是某中文版＋英文Corpfiles破解完成。

## 软件寿命结束

- 软件不再销售并已被停止维护与支持，如win7

## 最终用户许可协议eula

- eula(End User Licence Agreement):最终用户许可协议，指一家公司的软件与软件的使用者所达成的协议.

```shell
如C:\Program Files\Microsoft Office\root\Office16\2052\AccessRuntime_eula.txt中的内容的最后有一行EULAID，就是你的版本。

EULAID:O16_RTM_ART.1_RTM_CN

如简体中文正式版是EULAID:WX.4_PRO_RTL_CN，繁体中文正式版是 WX.4_PRO_RTL_TW。其中:如果是WX.开头是正式版，WB.开头是测试版。_PRE，代表家庭版；_PRO，代表专业版。
```

# 版本简写

## 按授权和功能划分

Trial:试用版，通常都有时间限制，有些试用版软件还在功能上做了一定的限制

Unregistered:未注册版，通常没有时间限制，在功能上相对于正式版做了一定的限制

Regged:已注册版

Demo:演示版，仅仅集成了正式版中的几个功能，不能升级成正式版

Lite:精简版

Full version:完整版，属于正式版

## 按语言划分

SC:Simplified Chinese简体中文版

CN:简体中文版

GBK:简体中文汉字内码扩展规范版。

TC:Traditional Chinese繁体中文版

CHT:繁体中文版

BIG5:繁体中文大五码版。

EN:英文版

Multilanguage:多语言版

UTF8:Unicode Transformation Format 8bit，对现有的中文系统不是好的解决方案。

## 其他版本

Preview:预览版

Express:简易版

Mini:迷你版/精简版,只有最基本的功能

Free:自由版

Standard:标准版

Enhance:增强版或者加强版　属于正式版1

Plus:属增强版，不过这种大部分是在程序界面及多媒体功能上增强。

Upgrade:升级版

Professional:专业版

Corporation&Enterprise:企业版


Premium:贵价版

Deluxe:豪华版

Cardware:属共享软件的一种，只要给作者回复一封电邮或明信片即可,有的作者提供注册码等

Rip :从原版文件（一般是指光盘或[光盘镜像](https://baike.baidu.com/item/光盘镜像)文件）直接将有用的内容（核心内容）分离出来，剔除无用的文档

# Code Review(审查)简写

1. **PR**: Pull Request. 拉取请求，给其他项目提交代码
2. **LGTM**: Looks Good To Me. 朕知道了 代码已经过 review，可以合并
3. **SGTM**: Sounds Good To Me. 和上面那句意思差不多，也是已经通过了 review 的意思
4. **WIP**: Work In Progress. 传说中提 PR 的最佳实践是，如果你有个改动很大的 PR，可以在写了一部分的情况下先提交，但是在标题里写上 WIP，以告诉项目维护者这个功能还未完成，方便维护者提前 review 部分提交的代码。
5. **PTAL**: Please Take A Look. 你来瞅瞅？用来提示别人来看一下
6. **TBR**: To Be Reviewed. 提示维护者进行 review
7. **TL , DR**: Too Long; Didn't Read. 太长懒得看。也有很多文档在做简略描述之前会写这么一句
8. **TBD**: To Be Done(or Defined/Discussed/Decided/Determined). 根据语境不同意义有所区别，但一般都是还没搞定的意思
9. **PRD** : Product Requirement Document. 产品需求文档
10. **TBH** ：to be honest  老实说
11. **IMAO** ：laugh my ass off 笑到不行，超爆笑
12. **BTW** ：by the way 顺带一提
13. **TTYL**：talk to you later 晚点聊
14. **IDK** ：l don't know 我不知道
15. **AKA**：as known as 也就是，以...为人所知
16. **plz**：please 拜托
17. **thx**：thanks 谢谢
18. **tmr**：tomorrow 明天
19. **ppl**：people 人们，大家
20. **IMHO**：in my humble opinion 依我浅见
21. **FAQ**:frequently asked questions常见问题
22. **DRY**:Don't repeat yourself不要自我重复

# 参考文献

[软件版本周期]([https://zh.wikipedia.org/wiki/%E8%BB%9F%E4%BB%B6%E7%89%88%E6%9C%AC%E9%80%B1%E6%9C%9F](https://zh.wikipedia.org/wiki/軟件版本週期))

[软件版本号规范与命名原则](https://www.jianshu.com/p/75374e299ef8)

[软件版本]([https://baike.baidu.com/item/%E8%BD%AF%E4%BB%B6%E7%89%88%E6%9C%AC](https://baike.baidu.com/item/软件版本))