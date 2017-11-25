# hexo-theme-lessless

[English](./README.md)
Hexo 主题，没有什么功能，就是简单的博客主题。

# Usage

进入 hexo 文件夹：

```shell
git clone git@github.com:zhengxiaowai/hexo-theme-lessless.git themes/lessless
```

额外的 hexo 配置:

```shell
npm install hexo-prism-plugin
npm install hexo-renderer-marked
```

复制以下内容到 hexo _config.yaml 中

```yaml
prism_plugin:
  mode: 'preprocess'    # realtime/preprocess
  theme: 'default'
  line_number: false    # default false

marked:
  gfm: true
  pedantic: false
  sanitize: false
  tables: true
  breaks: true
  smartLists: true
  smartypants: true
  modifyAnchors: ''
  autolink: true
```

关闭默认的 highlight

```yaml
highlight:
  enable: false
```

# lessless 配置

## menu

主题导航相关配置

```yaml
menu:
  首页: /
  分类: /categories
  归档: /archives
  # 标签: /tags 
  # 关于: /about

```

默认开启：首页、分类、归档

## busuanzi

简易的页面 uv、pv 的计算

```yaml
busuanzi:
  enable: true
```

默认开启会在首页底部显示 uv 和 pv，在文章页面的题目下方显示 pv

## disqus

disqus 评论设置

```yaml
disqus:
  enable: false
  shortname: <你的 shortname>
```