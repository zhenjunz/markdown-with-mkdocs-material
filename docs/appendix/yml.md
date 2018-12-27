```yaml
site_name: 第一个静态网页
site_description: 第一个静态网页
site_author: 作者
site_url: https://zhenjunz.github.io/markdown-with-mkdocs-material/

repo_name: 'markdown-with-mkdocs-material'
repo_url: 'https://github.com/zhenjunz/markdown-with-mkdocs-material'

theme:
  name: material
  palette:
    primary: 'Blue Grey'
    accent: 'Pink'
  feature:
    tabs: false
  #font:
    #text: 'Ubuntu'
    #code: 'Ubuntu Mono'
  language: 'zh'

extra:
  social:
    - type: github
      link: https://github.com/zhenjunz
  search:
    language: 'jp'

markdown_extensions:
  - admonition
  - codehilite:
      guess_lang: false
      linenums: false
  - toc:
      permalink: true
  - footnotes
  - meta
  - def_list
  - pymdownx.arithmatex
  - pymdownx.betterem:
      smart_enable: all
  - pymdownx.caret
  - pymdownx.critic
  - pymdownx.details
  - pymdownx.emoji:
      emoji_generator: !!python/name:pymdownx.emoji.to_png
      #emoji_generator: !!python/name:pymdownx.emoji.to_svg
      #emoji_generator: !!python/name:pymdownx.emoji.to_png_sprite
      #emoji_generator: !!python/name:pymdownx.emoji.to_svg_sprite
      #emoji_generator: !!python/name:pymdownx.emoji.to_awesome
      #emoji_generator: !!python/name:pymdownx.emoji.to_alt
  - pymdownx.inlinehilite
  - pymdownx.magiclink
  - pymdownx.mark
  - pymdownx.smartsymbols
  - pymdownx.superfences
  - pymdownx.tasklist
  - pymdownx.tilde

extra_javascript:
  - 'js/extra.js'
  - 'js/baidu-tongji.js'
  - 'https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.0/MathJax.js?config=TeX-MML-AM_CHTML'

nav:
  - 一. 介绍: index.md
  - 二. 安装:
      - 1. 本地环境搭建: install/local.md
      - 2. 发布至GitHub Pages: install/github-pages.md
      - 3. 发布至自己的HTTP Server: install/http-server.md
  - 三. 语法:
      - 1. 语法总览: syntax/main.md
      - 2. 标题: syntax/headline.md
      - 3. 段落: syntax/paragraph.md
```
