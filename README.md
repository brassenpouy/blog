# Blog

技术分析与行业洞察，托管于 GitHub Pages。

**访问地址**: https://brassenpouy.github.io/blog/

## 目录结构

```
blog/
├── index.html                  # 索引页（从 posts.json 自动渲染）
├── assets/
│   ├── index.css               # 索引页样式
│   ├── article.css             # 文章页共享样式
│   └── posts.json              # 文章元数据
├── <slug>/
│   ├── index.html              # GitHub Pages 版（外部 CSS + Mermaid JS）
│   └── wechat.html             # 微信公众号版（全内联样式，无 JS）
└── README.md
```

## 每篇文章两个版本

| 版本 | 文件 | 特点 | 用途 |
|------|------|------|------|
| GitHub Pages | `index.html` | 外部 CSS，Mermaid JS 渲染，响应式 | 即刻/社媒分享链接 |
| 微信公众号 | `wechat.html` | 全内联 style，无 JS，图表用纯 HTML | 复制粘贴到公众号编辑器 |

## 新增文章

1. 新建目录 `<slug>/`
2. 创建 `index.html`，`<head>` 中引用 `<link rel="stylesheet" href="../assets/article.css">`
3. 创建 `wechat.html`，所有样式内联，Mermaid 图替换为 HTML 结构化卡片
4. 在 `assets/posts.json` 中添加一条记录
5. `git push` 即自动部署

## 微信公众号发布流程

1. 在浏览器打开 `https://brassenpouy.github.io/blog/<slug>/wechat.html`
2. `Ctrl+A` 全选 → `Ctrl+C` 复制
3. 在公众号编辑器中 `Ctrl+V` 粘贴，格式自动保留
4. 微调图片和段间距后发布

## 内容来源

文章基于 AI-Brain Obsidian Vault 中的 `.md` 笔记生成，AI-Brain 仓库保持纯 Markdown 形式。
