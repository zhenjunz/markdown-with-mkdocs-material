虽然search功能(lunr.js)暂不直接支持中文，但测试发现设置为日语后，中文和英文搜索都可以使用

```text
extra:
  search:
    language: 'jp'
```

另外，搜索对话框的显示文字，默认为英文，可以设置为中文。例如"search"改为中文后就叫"搜索"

```text
theme:
  language: 'zh'
```
