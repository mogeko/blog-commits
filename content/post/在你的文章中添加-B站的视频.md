---
title: "在你的文章中添加 B站的视频"
date: 2017-09-09T18:00:00+08:00
draft: false
tags: ["Hexo"]
---

![Logo](https://mogeko.github.io/post/%E5%9C%A8%E4%BD%A0%E7%9A%84%E6%96%87%E7%AB%A0%E4%B8%AD%E6%B7%BB%E5%8A%A0-b%E7%AB%99%E7%9A%84%E8%A7%86%E9%A2%91/logo.png)
参考 <https://github.com/Z4Tech/hexo-tag-bilibili>

<!--more-->

# 准备工作

1. Node.js 这是一个 Hexo插件，所以通过 npm 安装。

# 正文

## 安装 hexo-tag-bilibili

这就是那个神奇的插件，名叫 hexo-tag-bilibili。
我们通过 npm 进行安装。
切换到 Hexo 的目录，执行一下命令

```
$ cd [你的 Hexo目录]
$ npm install --save hexo-tag-bilibili
```

![安装 hexo-tag-bilibili](https://mogeko.github.io/post/%E5%9C%A8%E4%BD%A0%E7%9A%84%E6%96%87%E7%AB%A0%E4%B8%AD%E6%B7%BB%E5%8A%A0-b%E7%AB%99%E7%9A%84%E8%A7%86%E9%A2%91/install_hexo-tag-bilibili.png)

## 使用

在文章中用一下方式使用此插件
[av_id] 填写视频的 av号。

```
{% bilibili [av_id] %}
```

如果有多 p，使用一下格式。[page] 为 P号。

```
{% bilibili [av_id] [page] %}
```

例如：

```
{% bilibili av2271112 %}
```

<embed height="415" width="544" quality="high" allowfullscreen="true" type="application/x-shockwave-flash" src="//static.hdslb.com/miniloader.swf" flashvars="aid=2271112&amp;p=1">

## 高级

### 配置

你可以配置你的播放器
在 Hexo 的文件夹中，打开 `_config.yml`文件进行配置。
你可以配置 是否`自动播放`，播放器的`大小` 等。
例如

```
bilibili:
  width: 452
  height: 544
```

### Style

播放器由一个带有 `bili_video` 类的 `<div>`标签包装。你可以通过自定义的 css文件修改它的样式。



<br>

<center>  ·End·  </center>