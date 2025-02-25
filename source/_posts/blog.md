---
title: blog搭建
tags:
  - Hexo
  - butterfly
categories: 博客搭建
abbrlink: e6a32f0a
date: 2025-02-07 10:05:59
---

这篇文章记录了简易博客的搭建过程。我使用的搭建工具是 Hexo，主题是 butterfly。
Hexo: https://hexo.io/
butterfly: https://butterfly.js.org/

## 安装 Hexo

```bash
$ pnpm install hexo -g
```

详细的安装方法: https://hexo.io/zh-cn/docs/

## 创建 Hexo 项目

### 创建文件夹 blog

### 初始化 Hexo

进入文件夹 blog，然后初始化 Hexo 项目

```bash
$ hexo init
$ pnpm install
```

## 安装 butterfly 主题

### 安装

```bash
$ pnpm install hexo-theme-butterfly
```

### 应用主题

修改 blog 根目录下的 \_config.yml，把主题改为 butterfly

```yaml
theme: butterfly
```

### 安装插件

```bash
$ pnpm install hexo-renderer-pug hexo-renderer-stylus
```

### 创建配置文件

在 blog 根目录下创建一个文件`_config.butterfly.yml`，并将`blog/node_modules/hexo-theme-butterfly/_config.yml`中的内容复制到`_config.butterfly.yml`中。

## 启动
```bash
$ pnpm run server
```
