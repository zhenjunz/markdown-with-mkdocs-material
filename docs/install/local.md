## **环境说明**

---

- python: 2.7.10

- 依赖的python包:

	| 包名 | 模块名 | 版本 |
	| :-- | :---- | :--  |
	| mkdocs | mkdocs | 0.16.3 |
	| mkdocs-material | material | 1.10.1 |
	| Markdown | markdown | 2.6.9 |
	| pymdown-extensions | pymdownx | 4.0 |

## **mkdocs-material部署**

---

- 安装

	```text
	pip install mkdocs mkdocs-material
	```

- 初始化项目

    ```text
    mkdocs new my-project
    ```

- 修改主题, mkdocs.yml里添加:

	```text
	theme: material
	```

- 添加扩展, mkdocs.yml里添加:

	```text
	markdown_extensions:
	    - admonition
	    - codehilite(guess_lang=false,linenums=false)
	    - toc(permalink=true)
	    - footnotes
	    - meta
	    - def_list
	    - pymdownx.arithmatex
	    - pymdownx.betterem(smart_enable=all)
	    - pymdownx.caret
	    - pymdownx.critic
	    - pymdownx.details
	    - pymdownx.emoji:
	        emoji_generator: !!python/name:pymdownx.emoji.to_png
	    - pymdownx.inlinehilite
	    - pymdownx.magiclink
	    - pymdownx.mark
	    - pymdownx.smartsymbols
	    - pymdownx.superfences
	    - pymdownx.tasklist
	    - pymdownx.tilde
	```

- [可选][添加百度统计](/appendix/baidu_tongji/)

- [可选][改变页面配色](/appendix/color/)

- mkdocs服务启动

    ```text
    cd my-project
    mkdocs serve
    ```

- 通过浏览器打开http://127.0.0.1:8000/，查看效果
