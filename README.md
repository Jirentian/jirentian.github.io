[Hux Blog](https://huangxuan.me)
================================

> 我从未想到它会变得如此受欢迎。

![](http://huangxuan.me/img/blog-desktop.jpg)


[用户手册 👉](_doc/Manual.md)
--------------------------------------------------

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
