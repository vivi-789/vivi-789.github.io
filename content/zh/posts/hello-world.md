---
title: "你好，世界"
weight: -100
date: 2026-06-18T10:00:00+08:00
draft: false
tags: ["hello", "getting-started"]
categories: ["tutorial"]
description: "欢迎来到你的新知识库！"
---

## 欢迎来到你的知识库

这是你的第一篇文章。你可以编辑或删除它，然后开始撰写自己的内容。

### 如何撰写新文章

1. 在 `content/zh/posts/` 目录下创建一个新的 `.md` 文件
2. 在文件顶部用 `---` 标记添加 front matter（元数据）
3. 使用 Markdown 语法撰写内容

### 基础 Markdown 语法

**加粗文字**：`**加粗**`

*斜体文字*：`*斜体*`
：`
`

> 引用：在行首使用 `>`

`行内代码`：用反引号包裹文字

```python
# 代码块
print("你好，世界！")
```

### 添加图片

将图片放入 `static/media/` 文件夹，然后像这样引用：

```markdown
```

或者使用 Obsidian 的拖拽功能 —— 图片路径会自动处理。

### 添加视频

对于托管在外部平台（YouTube、Bilibili 等）的视频，使用嵌入代码。

对于本地视频，将其放入 `static/media/` 并引用：

```html
<video controls src="/media/your-video.mp4"></video>
```

> ⚠️ **注意**：GitHub 单文件上限为 100MB。大型视频建议托管在外部平台，然后通过 iframe 嵌入。

### 添加音频

```html
<audio controls src="/media/your-audio.mp3"></audio>
```

### 控制文章可见性

若要使文章**不公开**（不发布），在 front matter 中设置 `draft: true`：

```yaml
---
title: "私密笔记"
date: 2026-06-18T10:00:00+08:00
draft: true  # 这篇文章将不会被发布
tags: []
---
```

---

祝你写作愉快！🎉
