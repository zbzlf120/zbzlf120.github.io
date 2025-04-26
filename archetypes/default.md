---
date: {{ .Date }}
draft: true
title: "{{ replace .File.ContentBaseName "-" " " | title }}"
tags:
  - Java
categories:
  - 后端开发
cover:
    image: "/pic/mybaties.png" # image path/url
    alt: "mybaties" # alt text
    caption: "mybaties" # display caption under cover
    relative: false # when using page bundles set this to true
    hidden: false # only hide on current single page
---
