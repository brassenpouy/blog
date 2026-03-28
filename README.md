# Blog

技术分析与行业洞察，托管于 GitHub Pages。

**访问地址**: https://brassenpouy.github.io/blog/

## 目录结构

```
blog/
├── index.html              # 索引页（自动从 posts.json 渲染列表）
├── assets/
│   ├── index.css           # 索引页样式
│   ├── article.css         # 文章共享样式（表格/卡片/callout/timeline…）
│   └── posts.json          # 文章元数据（索引页读取此文件）
├── <article-slug>/
│   └── index.html          # 文章页（引用 ../assets/article.css）
└── README.md
```

## 新增文章

1. 创建目录 `<slug>/index.html`
2. 在 `<head>` 中引用共享样式：`<link rel="stylesheet" href="../assets/article.css">`
3. 在 `assets/posts.json` 中添加一条记录
4. `git push` 即自动部署
