---
layout: post
title:  "lht的博客!"
date:   2016-10-27 11:52:52 +0800
categories: jekyll update
---




在Github上建立仓库

第一步，想在Github上建仓库库，你得有个Github账号，如果没有，那你就得注册一个账号，进入Github官网，填写注册信息，这些应该对你来说非常简单了，接着你会来到下图：

根据步骤点击，有了账号以后你需要对你的邮箱进行验证，一定要验证。

好了，现在我们终于可以建立仓库了，我们有两种方法：

    一种是用git命令，如果不会git命令，这里推荐一个学习的网站，相信它会对小白阶段的你有很大的帮助，虽然我也是一个小白Git教程
    在github网页上进行操作或者在github桌面工具中操作并上传

如果使用git命令，大致语句如下，根据自己账号名的不同进行更改

echo "# dapengyou.github.com" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/dapengyou/dapengyou.github.com.git
git push -u origin master

    如果没有绑定 SSH key，一般会要求输入用户名和密码

如果使用的是第二种方法,操作如图

接下来会会出现下图：

不需要勾选「Initialize this repository with a README」，当然你勾选了也可以，这个时候我们的仓库什么东西还没有, 所以我们还要初始化点东西, 点击右上角的settings, 在网页的最下面点击Launch automatic page generator, 然后一路继续

接下来会让你选择主题, 由于我们最后要自己上传网页, 所以这里默认就好, 直接点击publish pages下一步就可以了。

好了, 理论上现在你的个人博客就已经创建好了, 通过浏览器访问一下

    https://你的github帐号.github.io

这时你就可以看到一个默认生成的网页了，这时我们就可以安安心心的进入下一步了
使用jekyll模板

在之前的工作都完成后，你需要将仓库文件close到本地，close的语句：
git clone https://github.com/dapengyou/dapengyou.github.com.git

接着删掉里面的内容，进入jekyll网页模板中选择自己喜欢的模板下载，将下载的所有的内容复制到刚刚clone下来的文件夹中。

接下来，也是很重要的一点，因为克隆了别人的模板，所以在_config.yml文件中修改相应的信息，将模板变成自己的。

这里我用的模板是Jacman，所以更改的内容可以参照配置指南

不过重中之重是你的电脑里有配置jekyll。
提交仓库

终于到了最后一步，就是将你clone后并配置好的文件夹提交到远程仓库

这时再输入dapengyou.github.io,将会出现下图：

属于自己的博客就搭建好了

当然，还有一点小小的瑕疵，那就是要怎么样添加自己的文章呢？别急，往下看

在你下载的文件中有一个文件夹_post/，只需要在此文件夹中加入带有 YAML 头信息的 markdown 文件，然后 push 到 Github，就会被自动渲染成 HTML。

带有 YAML 头信息如下：

---
layout: post
title: 这里是题目
tags:
- 标签1
- 标签2
categories: 分类
description: 描述。
---

    这个YAML 头信息很重要，如果没有这个，就没有这么美观的网页了，你们也可以试试不加是什么效果哦







