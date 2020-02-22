<center><b><font color="b" size="7">About Github</font></b></center>
# [Github术语表](https://help.github.com/cn/github/getting-started-with-github/github-glossary)

- **git**: 一个开源的分布式版本控制系统
- **GitHub**: 一个托管和协作管理 Git 仓库的平台
- **repository:**版本库
- **star**:收藏，到收藏中心方便下次查找
- **fork派生/复刻**: a copy of a repository on GitHub owned by a different user，在自己的第三方平台远端，拷贝到远端
- **pull request拉取请求**: a place to 比较和讨论the differences introduced on a branch with reviews, comments, integrated tests, and more一个用于比较和讨论分支中引入的差异的地方，其中包含评论，评论，集成测试等
- **watch关注**:关注某个项目，之后若有更新，你会在第一时间收到更新通知
- **issue议题**:与仓库相关的建议改进、任务或问题。 议题可由任何人创建（对于公共仓库），由仓库协作者进行管理。 每个议题都包含自己的讨论论坛，可进行标记和分配给用户。
- **blame追溯**:Git 中的“追溯”功能描述文件中每一行的最后修改，通常显示修订、作者和时间信息。 例如，在跟踪导致故障的功能添加或导致特定漏洞的提交时，此功能非常有用。
- **check检查**:GitHub 上的一种状态检查类型
- **collaborator协作者**:协作者是受仓库所有者邀请参与,对仓库拥有读取和写入权限的人
- **contributor贡献者**:贡献者是指通过合并拉取请求为项目做出贡献，但没有协作者权限的人
- **dashboard仪表盘(个人/组织)**:个人仪表板是有关您在 GitHub 上的活动的信息中心。 通过个人仪表板，可跟踪您关注或参与的议题和拉取请求、导航到您的顶层仓库和团队页面，以及了解您关注或参与的仓库中的最近活动。 还可以发现新仓库，这些仓库根据您关注的用户和标注的仓库而推荐。 如果只查看特定组织的活动，请访问该组织的仪表板
- **diff差异**:两次提交或保存的更改之间的不同之处
- **enterprise account企业账户**:企业帐户允许您集中管理多个 GitHub.com 组织的策略和帐单。 企业帐户可用于 GitHub Enterprise Cloud。
- **organization组织**:组织是共享帐户，其中业务和开源项目可一次协助处理多个项目。 所有者和管理员可通过复杂的安全和管理功能管理成员对组织数据和项目的访问。
- **team团队**:通过级联访问权限和提及来反映公司或群组结构的组织成员组
- **SSH Key**:一种使用加密消息向在线服务器标识自己的方法
- **upstream上游**:在谈论分支或复刻时，原始仓库上的主分支通常被称为“上游”，因为它是获取其他更改的主要位置。 您正在处理的分支/复刻则被称为“下游”
- **commit提交**: 一个 Git 对象，a snapshot of your entire repository compressed into a SHA
- **branch分支**: 一个轻型可移动的 commit 指针
- **clone**: 一个仓库的本地版本，包含所有提交和分支
- **remote远端**: 一个 GitHub 上的公共仓库，所有小组成员通过它来交换修改
- **HEAD**: 代表你当前的工作目录。使用`git checkout` 可移动 HEAD 指针到不同的分支、标记(tags)或提交

# [创建GitHub Pages site](https://help.github.com/en/github/working-with-github-pages/creating-a-github-pages-site#creating-a-repository-for-your-site):静态网页

- GitHub Pages site在网上强制公开，请删除涉及个人敏感的信息。
- 如果site是一个独立的项目，则创建新仓库来存储site源代码。 
- 如果site与现有项目关联， 则需将site的源代码(`Markdown\html`)添加至repo中的 `gh-pages` 分支或 `master` 分支上的 `docs` folder
- 如果您创建的是project site，请决定要使用哪个发布源(哪个分支)。 如果您创建的是用户或组织站点，您必须将站点的source files存储在 `master` 分支上 
- 如果site's source files 位于默认发布源 —`master`分支（对于user/organization site）或 `gh-pages`（对于project  site）- 但您的站点未自动发布，请确保有一个拥有管理权限和verified email address的人已推送到默认发布源。

## 创建user/organization site

- 创建一个repo-,且repo_name必须为`<user_name>.github.io`或 `<organization>.github.io`

- repo中必须包含一个包含一个index.html（也可以是其他文件名，但必须.html后缀)，此site仅支持

  或 `index.md`,其中包含要显示在site主页上的内容

- 访问网址:https://user_name.github.io或者https://organization_name.github.io

  例如:https://ZakijxZ.github.io

![用户或组织site](AboutGithub.assets/image-20200213003428171.png)

## 创建project  site

- 必须先创建repo，repo_name无限制，但必须先创建user/organization site

- 如果你选择的publishing source already exists, navigate to the publishing source.如果不存在, create the publishing source.

  ![project site](AboutGithub.assets/image-20200213003327036.png)

- 在publishing source的root文件夹下，创建一个`index.md`文件，也可以是`index.html`，其中包含要显示在site主页上的内容

- 如果您使用的是非默认发布源for a project site，[请配置您的发布源](https://help.github.com/cn/articles/configuring-a-publishing-source-for-your-github-pages-site#choosing-a-publishing-source)

- 在settings页面下拉至【GitHub Pages】，点击【Choose a theme】可选择site的主题页面

![image-20200212033003994](AboutGithub.assets/image-20200212033003994.png)

- repo对应的网址:https://user_name.github.io/repo_name

  如:https://ZakijxZ.github.io/Matlab_Tutorial

## 后续

- 可以通过创建更多新文件来向站点添加更多页面。每个文件都可以在您的站点上以与发布源相同的目录结构使用。例如，如果您的project site发布源是`gh-pages`分支，同时你在该分支上创建了一个名为新文件，名为`/about/contact-us.md`，该文件 will be available at`https://.github.io//about/contact-us.md`

## 利用Framework快速搭建

- [GitHub Pages](https://pages.github.com/) +[ Hexo ](https://hexo.io/):强大的API,插件功能好
- [GitHub Pages](https://pages.github.com/) + [jekyll ](http://jekyll.com.cn/):支持[Markdown](https://daringfireball.net/projects/markdown/), [Liquid](https://github.com/Shopify/liquid/wiki), HTML & CSS,[About GitHub Pages and Jekyll](https://help.github.com/en/github/working-with-github-pages/about-github-pages-and-jekyll)

# Github访问过慢怎么办

国外ip在线检测网站: https://www.ipaddress.com/,无法访问的话,请另辟蹊径.

`github.com`网站位于美国旧金山,所以初始访问` github.com `时网络寻址会比较耗费时间,这也是网站打开速度慢的其中一个原因.

最初用户从浏览器中输入` github.com` 网址时,浏览器并不知道这个域名对应的真实` ip` 地址,先问问自己电脑认识不认识这个域名的门牌号,如果本机不认识会接着往上问,当地运行商也不认识这个域名的话,继续问上级,直到问出来 github.com 的门牌号是` 192.30.253.113 `为止! 

如此繁琐的问路过程被称之为 DNS 寻址,如果问路的时间都占用很久,那么访问网站的速度自然会很慢. 所以,如果我们直接告诉浏览器目的地,那么浏览器也就不会一步一步去费劲问路了,这在一定程度上也就优化了访问网站的速度.

```bash
$ ping github.com -c 3 #查看 github.com 网站的门牌号
PING github.com (192.30.253.113): 56 data bytes
64 bytes from 192.30.253.113: icmp_seq=0 ttl=41 time=405.924 ms 
64 bytes from 192.30.253.113: icmp_seq=1 ttl=41 time=346.654 ms 
64 bytes from 192.30.253.113: icmp_seq=2 ttl=41 time=345.485 ms 
--- github.com ping statistics --- 
3 packets transmitted, 3 packets received, 0.0% packet loss 
round-trip min/avg/max/stddev = 345.485/366.021/405.924/28.220 ms
```

正常来说,网站的主域名下会存在多个子域名,由这些域名组合在一起提供完整的服务. 而 github.com 也不例外,其中 github.com是一级域名,也是主域名,其他的域名基本上都是二级域名或者说次域名. 所以我们不仅要告诉本机 github.com 的主域名,还要把相关的子域名也告诉本机,帮人帮到底,送福送到西!

 那到哪里去查询域名和 ip 的对应关系呢? 想一想现实生活中,每个人都有自己的家,而这个家有具体的地址,也就是平时说的门牌号. 

当然,有些人名下不只有一个家,有钱人的世界可以有很多家,毕竟狡兔还有三窟呢! 在这个家中既可以是单身窝,也可以是情侣房,或者是家庭房,具体容纳几个人是由房屋大小决定的. 

对应到计算机世界中,如果域名是用户,那么 ip 地址就是用户的家.

 同一个域名可以对应多个 ip 地址,同一个 ip 地址也可以有多个域名.

 如果有人想要拜访您,肯定要有具体的地址才能到你家里做客,从你家到你家的地址这个过程可能是你告诉他的,也可能是他自己找别人打听到的消息. 

域名到` ip` 地址的过程同样也需要找人询问,这个信息一般会存在 `dns `服务商那里,就像我们的地址登记到相关政府机构一样. 虽然相关机构的信息比较权威及时,但门槛有点高,所以不访问一下当地的"消息通".

 

互联网上的"消息通"更是数不胜数,这里推荐两个查询域名解析的网站.

https://www.ipaddress.com/

http://tool.chinaz.com/dns/

[域名相关](https://blog.csdn.net/qq_38071429/article/details/80339091)

我的机器上ping www.baidu.com和ping baidu.com得到的IP，不同地区ping同一个域名的IP地址可能不同

![img](https://img-blog.csdn.net/20180516172835777)

![img](https://img-blog.csdn.net/20180516172446107)

## 子域名有哪些

![image-20200213184305654](AboutGithub.assets/image-20200213184305654.png)



根据查到的相关域名信息,挨个挨个点,再次查询出这些域名对应的 ip 地址,于是整理出以下内容



```bash
#github related website 
192.30.253.113 github.com 
151.101.185.194 github.global.ssl.fastly.net 
192.30.253.118 gist.github.com 
192.30.253.120 codeload.github.com 
185.199.108.153 desktop.github.com 
185.199.108.153 guides.github.com 
185.199.108.153 blog.github.com 
18.204.240.114 status.github.com 
185.199.108.153 developer.github.com 
185.199.108.153 services.github.com 
192.30.253.175 enterprise.github.com 
34.195.49.195 education.github.com 
185.199.108.153 pages.github.com 
34.196.237.103 classroom.github.com
```



## 就近cdn加速

大型网站服务器都不会是只有一台服务器,而是多台服务器组成的集群一起对外提供服务.

 全世界都在使用 github ,如果每一次访问网站时走的都是美国服务器,即使浏览器知道目的地,但是距离太多遥远还是会很慢. 

因此,如果能够就近访问 github 网站就能大幅提高访问速度了,幸运的是,网络上同样有现成的工具来帮助我们查看就近的网站地址.

![github-speedup-chinaz-dns.png](https://snowdreams1006.tech/github/images/github-speedup-chinaz-dns.png)

从上图中我们可以看出,同一个域名有很多不同的 ip 地址,从中选择 `TTL（Time-To-Live的简称）` 值最小的作为优化标准. 于是,将上述清单继续优化成以下内容:

于是,将上述清单继续优化成以下内容,一条一条的查

```bash
# github related website 
192.30.253.113 github.com 
151.101.185.194 github.global.ssl.fastly.net 
203.98.7.65 gist.github.com 
13.229.189.0 codeload.github.com 
185.199.109.153 desktop.github.com 
185.199.108.153 guides.github.com 
185.199.108.153 blog.github.com 
18.204.240.114 status.github.com 
185.199.108.153 developer.github.com 
185.199.108.153 services.github.com 
192.30.253.175 enterprise.github.com 
34.195.49.195 education.github.com 
185.199.108.153 pages.github.com 
34.196.237.103 classroom.github.com
```

> 最好亲自测试一下就近站点以求获得最佳体验,不过推测应该差异不是很大,所以直接复制也无妨.

## 配置映射文件

### 对于windows

映射文件存放于:` C:\Windows\System32\drivers\etc\hosts`

- 打开 hosts 文件,将上述映射关系追加到文件末尾,保存并退出，每次更改前可先备份hosts文件
- 如果由于权限不足,无法保存,可以复制到桌面再编辑文件,最后移动并替换到 hosts 文件
- 运行 ipconfig /flushdns 刷新 dns 缓存.



### 对于mac 

映射文件存放于: `/etc/hosts `

- 编辑 hosts 文件并追加上述映射关系.
- 运行 sudo dscacheutil -flushcache 刷新 dns 缓存.

本文讲述了如何解决 github.com 网站访问速度慢的问题,通过修改本机的 hosts 文件来绕过 dns 解析,这种方法仅仅适用于能够访问网站只不过是访问速度慢这一现象. 如果本身无法访问国外网站,那么这种方法就不适用,可能需要另辟蹊径!

# Github 徽章从何而来



作者: 雪之梦技术驿站 链接: https://snowdreams1006.github.io/markdown/ 来源: 雪之梦技术驿站 本文原创发布于「雪之梦技术驿站」,转载请注明出处,谢谢合作!