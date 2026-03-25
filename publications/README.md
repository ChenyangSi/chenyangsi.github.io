# Publications

在这个文件夹里，每个 `.md` 文件对应一篇论文，`publications.html` 会在浏览器里读取这些文件的 front matter 并自动渲染。

建议直接复制任意一个现有文件作为模板，字段格式如下：

```md
---
title: 论文标题
authors: 作者列表，可用 **名字** 高亮
venue: 会议或期刊名称
year: 2025
group: 2025
image: ./assets/img/example.webp
alt: 图片替代文本
badges: CVPR 2025|default;Oral|highlight
links: PDF|https://example.com/paper.pdf;Code|https://github.com/example/repo
---
```

说明：

- `group` 决定显示在哪个折叠分组里，比如 `2025`、`2024`、`Earlier`
- `badges` 用分号分隔多个标签，格式是 `文字|样式`
- `links` 用分号分隔多个链接，格式是 `按钮名|URL`
- 页面顺序由 `assets/js/publications.js` 里的 `publicationFiles` 数组决定
