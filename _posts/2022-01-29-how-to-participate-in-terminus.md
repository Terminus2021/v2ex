---
layout: post
title:  【置顶】如何协助参与V2EX搬运计划
date:   2022-01-29
categories: Special
tags: Special
description: V2EX搬运计划，是在 GitHub 开放平台搭建的一个站点，以去中心化的方式搬运并备份V2EX论坛帖子。
is_sticky: true
---
## V2EX搬运计划是什么

V2EX搬运计划，是在 GitHub 开放平台搭建的一个站点，用于搬运并备份V2EX论坛文章。  
2022年1月发起，以向墙内搬运V2EX论坛文章为主。

## 抵抗屏蔽，需要V友参与新方法

在严重依赖微信、朋友圈的情况下，抵抗屏蔽，保证文章传播阅读的持久有效性，现在比较常见的方法有：

- 订阅号菜单栏的非正式群发
- 订阅号小号
- 文字保存为长图片
- 借助有道云笔记

可以发现，这些备份方法并没有很好地使用超链接、微信之外的网站平台，它们有时候也会意想不到的消失，就像断断续续的水滴。

V站的朋友参与抵抗屏蔽，需要开辟新的方法，重新捡起超链接、网站，再加上开源开放的协作平台。

V2EX搬运计划正是出于这样的原因与目的而产生。

## 如何参与V2EX搬运计划

### 需要的基本技能

- 熟悉使用 Markdown 基本标记语法
- 熟悉 Markdown 文本编辑器（可选项）：这些工具适用于对 Markdown 语法不熟悉的协作者
  - [MarkdownPad](http://markdownpad.com/)
  - [Atom](https://atom.io/)
  - html 转成 markdown：浏览器插件「[简悦](http://ksria.com/simpread/)」
- 熟悉 GitHub 平台使用

### PR 步骤说明

1. 注册并登录 [GitHub](https://github.com/) 帐号

2. fork v2ex 仓库到自己的 GitHub: 访问[计划](https://github.com/Terminus2021/v2ex) GitHub页面，点击右上角 **Fork** 按钮。

3. 认领备份：查看[备份 issues](https://github.com/Terminus2021/v2ex/issues)，在标记为 help-wanted 的 issue 中发布评论，表示认领该文章搬运。

4. 编辑文章备份：在自己帐号里面的 v2ex 仓库，编辑添加备份的文章。

    - 第一种方式：直接在线编辑添加
      1. 点击进入 `_posts/` 文件夹，点击上面的 **Create New File**
      2. 命名文章标题：统一格式为「Year-Month-Day-title.md」，例如 `2018-01-01-biao-ti.md`
      3. 在下方 **Edit new file** 空白区域编辑内容，编辑格式看下方[备份格式编辑要求](#备份格式编辑要求)
      4. 点击 **Preview** 可预览效果
        ![add_new_post.png](https://i.loli.net/2020/02/09/uhZUAWm6yr3MJ4I.png)

    - 第二种方式：从本地上传已编辑的 md 文档
      1. 点击进入 `_posts/` 文件夹，点击 **Upload files**
        ![drag_files.png](https://i.loli.net/2020/02/09/Be21nogCdw4pJlE.png)
      2. 从本地选择要上传的 md 文档

5. 填写 **commit new file**
  ![commit_new_file.png](https://i.loli.net/2020/02/09/fCs72X3pBYgSkT8.png)

6. 向原仓库提交 PR
    
    在自己的仓库页面，点击 **new pull request**，再点击 **create pull request**，填写 PR 描述并提交。
    ![new_pull_request.png](https://i.loli.net/2020/02/09/mONEWGFJwXod1ep.png)

7. 等待 Terminus2021 查看 PR ，符合要求的内容会 merge(合并）。

### 备份格式编辑要求

1. 头部格式：

    ```
    ---
    layout: post
    title:  ❤Introduce Project Babel 2.0
    date:   2018-04-09
    categories: 技术
    tags: V2EX
    image_feature: ""
    description: 
    ---
    ```
    - layout: post 保持不变
    - title: 用备份文章的标题
    - date: 被删日期
    - categories: 分类
    - tags: 节点（在V2EX查看是否已有相关节点）
    - image_feature: "如果文章有合适的图片可作为封面图，图片链接填在这里，若无则不填写"
    - description: 可用文章的导语做简述

2. 正文小标题，使用 h2 或 h3。

3. 图片编辑
  1. 使用 [https://sm.ms](https://sm.ms) 或 [https://imgur.com](https://imgur.com) 图床平台生成链接。
  2. 图注用 `<center>图注</center>` 居中。
