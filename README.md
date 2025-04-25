指导网站:https://gohugo.io/getting-started/quick-start/

1. 打开windows powershell

2. winget search Microsoft.PowerShell

3. winget install --id Microsoft.PowerShell --source winget

4. winget install Hugo.Hugo.Extended

启动
  hugo new site myrecord-hugo
  cd myrecord-hugo
  git init
  git submodule add https://gitee.com/nism-github/gohugo-theme-ananke.git themes/ananke
  echo "theme = 'ananke'" >> hugo.toml
  hugo server
  
5.创建文章

hugo new content content/posts/redis01.md

启动
hugo server   
hugo --buildDrafts    # or -D
hugo --buildExpired   # or -E
hugo --buildFuture    # or -F
发布-不包括  draft, future, or expired content 内容
hugo
帮助命令hugo help
创建不同的配置文件: hugo --config other.toml 或者  hugo --config a.toml,b.yaml,c.json


title: "文章标题"
date: 2024-03-21
draft: false
tags: ["Java", "Spring"]
categories: ["后端开发"]
description: "这是文章描述"
weight: 1
cover:
    image: "cover.jpg"    # 封面图片
    alt: "封面图片描述"
    caption: "图片标题"
