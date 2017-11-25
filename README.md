# hexo-theme-lessless

[中文](./README-zh.md) 
the simple theme for hexo. which has no futures, just very simple. 

# Usage

enter hexo folder and git clone lessless：

```shell
git clone git@github.com:zhengxiaowai/hexo-theme-lessless.git themes/lessless
```

extra hexo config:

```shell
npm install hexo-prism-plugin
npm install hexo-renderer-marked
```

copy the content below to hexo's _config.yml

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

close default highlight:

```yaml
highlight:
  enable: false
```

# lessless theme config

## menu

about top navs


```yaml
menu:
  Home: /
  Categotry: /categories
  Archive: /archives
  # Tag: /tags 
  # About: /about 
```

default enable：Home、Category、Archive


## busuanzi

Simple calculation for pv(uv)

```yaml
busuanzi:
  enable: true
```

show pv and uv under home page and show pv under post's title when enable busuanzi

## disqus

disqus comment config

```yaml
disqus:
  enable: false
  shortname: <your_shortname>
```