# 我本平凡 - 个人博客

这是一个基于Jekyll的个人博客，用于分享留学、语言学习、AI技术、工作和海外生活的经历和思考。

## 特点

- 简洁的设计风格
- 支持Markdown写作
- 包含博客文章和周刊栏目
- 托管在GitHub Pages上

## 本地开发

### 前提条件

- Ruby 2.5.0 或更高版本
- RubyGems
- GCC 和 Make

### 安装步骤

1. 安装Jekyll和Bundler

```bash
gem install jekyll bundler
```

2. 克隆仓库

```bash
git clone https://github.com/yourusername/yourusername.github.io.git
cd yourusername.github.io
```

3. 安装依赖

```bash
bundle install
```

4. 启动本地服务器

```bash
bundle exec jekyll serve
```

5. 在浏览器中访问 http://localhost:4000

## 写作指南

### 创建新文章

在 `_posts` 目录下创建新的Markdown文件，文件名格式为 `YYYY-MM-DD-title.markdown`。

文章头部需要包含以下Front Matter：

```yaml
---
layout: post
title:  "文章标题"
date:   YYYY-MM-DD HH:MM:SS +0100
categories: blog
---
```

### 创建新周刊

在 `_posts` 目录下创建新的Markdown文件，文件名格式为 `YYYY-MM-DD-weekly-XX.markdown`，其中XX为期数。

周刊头部需要包含以下Front Matter：

```yaml
---
layout: post
title:  "周刊 #XX：标题"
date:   YYYY-MM-DD HH:MM:SS +0100
categories: weekly
---
```

## 部署到GitHub Pages

1. 创建一个名为 `yourusername.github.io` 的GitHub仓库
2. 将本地仓库推送到GitHub

```bash
git add .
git commit -m "Initial commit"
git push -u origin main
```

3. 在GitHub仓库设置中启用GitHub Pages
4. 访问 `https://yourusername.github.io` 查看你的博客

## 自定义

- 修改 `_config.yml` 文件中的个人信息和社交链接
- 修改 `about.markdown` 文件中的个人介绍
- 自定义主题样式可以通过创建 `assets/css/style.scss` 文件实现

## 许可证

[MIT](LICENSE)