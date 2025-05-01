[Hux Blog](https://huangxuan.me)
================================

> 我从未想到它会变得如此受欢迎。

![](http://huangxuan.me/img/blog-desktop.jpg)


[用户手册 👉](_doc/Manual.md)
--------------------------------------------------

## 目录
- [入门指南](#入门指南)
- [开发（从源码构建）](#开发从源码构建)
- [项目结构](#项目结构)
- [其他资源](#其他资源)
- [许可证](#许可证)

### 入门指南

1. 你需要安装 [Ruby](https://www.ruby-lang.org/en/) 和 [Bundler](https://bundler.io/) 来使用 [Jekyll](https://jekyllrb.com/)。按照 [使用Bundler和Jekyll](https://jekyllrb.com/tutorials/using-jekyll-with-bundler/) 的指南完成环境需求。

2. 安装 `Gemfile` 中的依赖：

```sh
$ bundle install 
```

3. 启动网站服务（默认地址为 `localhost:4000`）：

```sh
$ bundle exec jekyll serve  # 或者使用 npm start
```

### 开发（从源码构建）

要修改主题，你需要 [Grunt](https://gruntjs.com/)。在 `Gruntfile.js` 中有许多任务，包括压缩JavaScript、将 `.less` 编译为 `.css`、添加横幅以保持Apache 2.0许可证完整、监视更改等。

是的，这些都是继承而来并且极其老式的。没有模块化和转译等功能。

关键的Jekyll相关代码位于 `_include/` 和 `_layouts/` 中。它们大多是 [Liquid](https://github.com/Shopify/liquid/wiki) 模板。

这个主题使用Jekyll默认的代码语法高亮器 [Rouge](http://rouge.jneen.net/)，它与Pygments主题兼容，所以只需选择任何pygments主题的css（例如从[这里](http://jwarby.github.io/jekyll-pygments-themes/languages/javascript.html)）并替换 `highlight.less` 的内容即可。


### 想了解更多？查看[完整用户手册](_doc/Manual.md)！

### 项目结构

```
.
├── _config.yml               # 主配置文件：配置博客标题、描述、作者信息、社交链接等核心设置
├── _data                     # 数据文件：存储可重用的数据结构，如导航菜单、标签列表等
├── _doc                      # 文档目录：存放项目相关的使用说明文档
│   └── Manual.md             # 完整用户手册：提供详细的博客配置和使用指南
├── _drafts                   # 草稿文章：存放尚未发布的文章草稿
├── _includes                 # 页面组件：存放可复用的HTML片段和组件
│   ├── about                 # 关于页面组件：关于页面使用的特定组件
│   ├── footer.html           # 页脚组件：网站底部显示的内容，包括版权信息等
│   ├── head.html             # HTML <head>部分：包含元数据、CSS引用和站点设置
│   ├── header.html           # 页头组件：网站顶部导航栏和标题区域
│   └── ...                   # 其他组件：其他可复用的页面部分
├── _layouts                  # 布局模板：定义不同类型页面的整体结构
│   ├── default.html          # 默认布局：网站的基础HTML结构
│   ├── page.html             # 页面布局：普通内容页面的布局结构
│   ├── post.html             # 文章布局：博客文章的特定布局，包含文章元数据和分享功能
│   └── ...                   # 其他布局：其他特定用途的页面布局
├── _posts                    # 博客文章目录：存放所有已发布的博客文章，按日期命名
├── _site                     # 生成的静态网站：Jekyll构建后生成的完整静态网站文件
├── css                       # 样式文件：存放编译后的CSS样式表
├── fonts                     # 字体文件：博客使用的自定义字体文件
├── img                       # 图片资源：存放博客使用的所有图片资源
├── js                        # JavaScript文件：网站的交互功能脚本
├── less                      # Less样式源文件：预处理CSS的源文件，构建时编译为CSS
├── feed.xml                  # RSS订阅：允许读者通过RSS阅读器订阅博客
├── Gemfile                   # Ruby依赖定义：列出Jekyll及其插件的依赖关系
├── Gruntfile.js              # Grunt任务配置：定义自动化任务，如编译Less、压缩JS等
├── index.html                # 网站首页：博客的主页面，显示文章列表和介绍
├── package.json              # npm依赖和脚本：定义前端依赖包和可用的npm脚本命令
└── README.md                 # 项目说明文档：提供项目概述、安装和使用说明
```

其他资源
---------------

移植版本
- [**Hexo**](https://github.com/Kaijun/hexo-theme-huxblog) by @kaijun
- [**React-SSR**](https://github.com/LucasIcarus/huxpro.github.io/tree/ssr) by @LucasIcarus

[入门模板](https://github.com/huxpro/huxblog-boilerplate)
- 已过时。需要帮助更新到与主仓库相同的水平

翻译
- [🇨🇳  中文文档（有点过时）](https://github.com/Huxpro/huxpro.github.io/blob/master/_doc/README.zh.md)


许可证
-------

Apache License 2.0.
Copyright (c) 2015-present Huxpro

Hux Blog 衍生自 [Clean Blog Jekyll Theme (MIT License)](https://github.com/BlackrockDigital/startbootstrap-clean-blog-jekyll/)
Copyright (c) 2013-2016 Blackrock Digital LLC.
