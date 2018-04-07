---
title: Hello Hexo
categories: 写点啥
tags: [hexo]
---
感觉现在的自己有点舍本逐末了，大多数的时间都在搜索资料，反而消化知识的时间却没有多少（懒癌一枚了）。每每看到知乎和B站的收藏夹都心下暗念，一定要抽个时间来看看。可时间久了，也只是收藏的内容愈多，想看的心愈平淡了，所以搭建个自己的博客，记录自己的收获。同时也不想再为同样的问题花费时间成本了。
<!--more-->

# 正文：搭建与优化

>hexo的搭建与优化，网上已经有很多了，本篇就不赘述了，主要是想记录自己的优化的历程及遇到的一些问题（备份用）

## 博客搭建&&优化:
### 搭建
主要参考如下博文：
1: [搭建属于自己的博客](https://www.jianshu.com/p/465830080ea9)
2: [搭建 Hexo 博客--增强篇](https://www.jianshu.com/p/2640561e96f8)
3: [GitHub Pages + Hexo搭建个人博客](https://freeshow.github.io/Comprehensive/BuildBlog/GitHub%20Pages%20+%20Hexo%E6%90%AD%E5%BB%BA%E4%B8%AA%E4%BA%BA%E5%8D%9A%E5%AE%A2/)


### 优化
> * [Gulp压缩](http://luckykun.com/work/2016-07-10/hexo-faster.html?utm_source=tuicool&utm_medium=referral)-压缩hexo的静态文件来提高访问速度[1]
> * [图片的问题](https://leaferx.online/2017/06/16/use-gulp-to-minimize/)-较方便的管理博客使用到的图片
> * [球状标签云](http://www.netcan666.com/2015/12/15/Hexo%E4%B8%AA%E6%80%A7%E5%8C%96%E7%90%83%E5%BD%A2%E6%A0%87%E7%AD%BE%E4%BA%91/)-比较炫酷

### 一些命令
> * hexo卸载 : npm uninstall hexo
> * 插件安装：npm install 插件名 --save
> * 插件卸载：npm uninstall 插件名
> * 插件更新：npm update

### 我的插件
在hexo目录下的package.json里可以看到hexo安装的插件
```
{
  "name": "hexo-site",
  "version": "0.0.0",
  "private": true,
  "hexo": {
    "version": "3.7.0"
  },
  "dependencies": {
    "hexo": "^3.2.0",
    "hexo-asset-image": "git+https://github.com/CodeFalling/hexo-asset-image.git",
    "hexo-deployer-git": "^0.3.1",
    "hexo-generator-archive": "^0.1.4",
    "hexo-generator-category": "^0.1.3",
    "hexo-generator-feed": "^1.2.2",
    "hexo-generator-index": "^0.2.0",
    "hexo-generator-search": "^2.2.5",
    "hexo-generator-sitemap": "^1.2.0",
    "hexo-generator-tag": "^0.2.0",
    "hexo-renderer-ejs": "^0.3.0",
    "hexo-renderer-marked": "^0.3.0",
    "hexo-renderer-stylus": "^0.3.1",
    "hexo-server": "^0.2.0"
  },
  "devDependencies": {
    "gulp-babel": "^7.0.1",
    "gulp-htmlclean": "^2.7.22",
    "gulp-htmlmin": "^4.0.0",
    "gulp-minify-css": "^1.2.4",
    "gulp-uglify": "^3.0.0"
  }
}
```
[1]: http://ngudream.com/2017/01/24/n-hexo-blog/