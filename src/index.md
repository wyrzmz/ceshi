---
# https://xiaotaokh.github.io/blog

# 页面的布局, home 主页的特殊布局  doc 默认文档样式 page 自定义布局
layout: home

# 当 layout 设置为 home 时，定义主页顶部的内容
hero:
  name: "wangyanru"
  text: "vitePress"
  tagline: 我的伟大项目标语
  image:
    src: /assets/home/home.jpeg
    alt: VitePress
  actions:
    - theme: brand
      text: Markdown 示例
      link: /views/examples/exp
    - theme: alt
      text: API 示例
      link: /views/examples/exp

# 当 layout 设置为 home 时，定义主页底部特色内容
features:
  - icon: icon-gongneng-copy  # 图标
    title: 特征 A  # 标题
    details: Lorem ipsum dolor sit amet, consectetur adipiscing elit  # 详情
    link: /views/examples/exp # 外部内部链接
    linkText: 更多 # 链接提示
    
  - title: 功能 B
    details: Lorem ipsum dolor sit amet, consectetur adipiscing elit
  - title: 功能 C
    details: Lorem ipsum dolor sit amet, consectetur adipiscing elit
---

<script setup>
import { useData } from 'vitepress';

const { theme, page, frontmatter } = useData()
</script>

[//]: # (<pre>{{ frontmatter }}</pre>)
<i class="iconfont icon-gongneng-copy"></i>

<style lang="scss">
  :root {
    --vp-home-hero-name-color: transparent;
    --vp-home-hero-name-background: -webkit-linear-gradient(120deg, #bd34fe, #41d1ff);
  }
</style>

1. [Link to baidu](https://www.baidu.com){target="_self"}
2. [Link to baidu_外部](https://www.baidu.com){target="_bink"}




1. [Home](/) <!-- 将用户导航至根目录下的 index.html -->
2. [foo](views/examples/exp) <!-- 将用户导航至目录 foo 下的 index.html -->

| Tables        |      Are      |  Cool |
| ------------- | :-----------: | ----: |
| col 3 is      | right-aligned | $1600 |
| col 2 is      |   centered    |   $12 |
| zebra stripes |   are neat    |    $1 |

> 1. :tada:
> 2. :100:


[[toc]]

::: info
这是一个信息框。
:::


```js:line-numbers {1}
// 启用行号
const line2 = 'This is line 2'
const line3 = 'This is line 3'
```









