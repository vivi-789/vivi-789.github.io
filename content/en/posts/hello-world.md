---
title: "Hello World"
date: 2026-06-18T10:00:00+08:00
draft: false
tags: ["hello", "getting-started"]
categories: ["tutorial"]
description: "Welcome to your new knowledge base!"
---

## Welcome to Your Knowledge Base

This is your first post. You can edit or delete it, and start writing your own content.

### How to Write a New Post

1. Create a new `.md` file in the `content/posts/` directory
2. Add the front matter (metadata) at the top between `---` markers
3. Write your content using Markdown

### Basic Markdown Syntax

**Bold text**: `**bold**`

*Italic text*: `*italic*`

[Link](https://example.com): `[Link](https://example.com)`

> Blockquote: Start a line with `>`

`Inline code`: Wrap text with backticks

```python
# Code block
print("Hello, World!")
```

### Adding Images

Place images in the `static/media/` folder, then reference them like this:

```markdown
![Image description](/media/your-image.png)
```

Or use Obsidian's drag-and-drop feature — the image path will be handled automatically.

### Adding Videos

For videos hosted on external platforms (YouTube, Bilibili, etc.), use the embed code.

For local videos, place them in `static/media/` and reference them:

```html
<video controls src="/media/your-video.mp4"></video>
```

> ⚠️ **Note**: GitHub has a 100MB per-file limit. Large videos should be hosted externally and embedded via iframe.

### Adding Audio

```html
<audio controls src="/media/your-audio.mp3"></audio>
```

### Controlling Post Visibility

To make a post **private** (not published), set `draft: true` in the front matter:

```yaml
---
title: "Private Note"
date: 2026-06-18T10:00:00+08:00
draft: true  # This post will NOT be published
tags: []
---
```

---

Happy writing! 🎉
