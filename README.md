# My Knowledge Base

基于 **Hugo + PaperMod 主题 + GitHub Pages** 构建的个人知识库。

---

## 目录结构

```
my-knowledge-base/
├── .github/workflows/     # GitHub Actions 自动部署配置
├── archetypes/            # 文章模板
├── assets/                # 需要 Hugo 处理的资源（SCSS、JS 等）
├── content/               # 网站内容
│   ├── posts/             # 英文文章
│   ├── zh/posts/          # 中文文章
│   ├── about/             # 英文关于页面
│   └── zh/about/          # 中文关于页面
├── data/                  # 数据文件
├── layouts/               # 自定义 HTML 模板
├── static/                # 静态文件（图片、视频、音频等）
│   └── media/             # 多媒体文件存放处
├── themes/PaperMod/       # Hugo 主题
├── config.yml             # Hugo 站点配置
└── README.md              # 本文件
```

---

## 快速开始

### 1. 注册 GitHub 账号

如果你还没有 GitHub 账号，前往 [github.com](https://github.com) 免费注册。

### 2. 创建 GitHub 仓库

1. 登录 GitHub，点击右上角 **+** → **New repository**
2. 仓库名填写：`<your-username>.github.io`
   - 例如：如果你的 GitHub 用户名是 `john`，仓库名就是 `john.github.io`
3. 选择 **Public**（公开仓库，免费）
4. 不要勾选 "Initialize this repository with a README"
5. 点击 **Create repository**

### 3. 修改配置文件

打开 `config.yml`，替换以下占位符：

| 占位符 | 替换为 |
|--------|--------|
| `<your-github-username>` | 你的 GitHub 用户名 |
| `Your Name` | 你的姓名 |
| `your-email@example.com` | 你的邮箱 |

### 4. 推送到 GitHub

在项目根目录下执行：

```bash
cd ~/my-knowledge-base
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/<your-username>/<your-username>.github.io.git
git push -u origin main
```

### 5. 启用 GitHub Pages

1. 打开 GitHub 仓库页面
2. 点击 **Settings** → **Pages**
3. **Source** 选择 "Deploy from a branch"
4. **Branch** 选择 "gh-pages" → "/ (root)"
5. 点击 **Save**

大约 1-2 分钟后，访问 `https://<your-username>.github.io` 即可看到你的网站！

---

## 写作流程

### 方式一：使用 Obsidian（推荐，非技术友好）

1. **安装 Obsidian**：从 [obsidian.md](https://obsidian.md) 下载免费版
2. **打开仓库**：在 Obsidian 中选择 "Open folder as vault"，选择 `~/my-knowledge-base`
3. **创建新文章**：
   - 在 `content/posts/` 目录下新建 `.md` 文件（英文）
   - 或在 `content/zh/posts/` 目录下新建 `.md` 文件（中文）
4. **Front matter 模板**：
   ```yaml
   ---
   title: "文章标题"
   date: 2026-06-18T10:00:00+08:00
   draft: false           # true = 不发布（私密），false = 发布（公开）
   tags: ["tag1", "tag2"] # 标签，方便分类检索
   categories: ["category"]
   description: "文章摘要"
   ---
   ```
5. **添加图片**：直接拖拽图片到 Obsidian，图片会自动存入 `static/media/`
6. **发布**：保存文件后，执行以下命令推送到 GitHub：
   ```bash
   cd ~/my-knowledge-base
   git add .
   git commit -m "Add new post"
   git push
   ```
   GitHub Actions 会自动构建并部署，约 1 分钟后网站更新。

### 方式二：使用任何文本编辑器

直接编辑 `.md` 文件即可，Markdown 语法通用。

---

## 添加多媒体

### 图片

将图片放入 `static/media/`，然后在文章中引用：

```markdown
![图片描述](/media/your-image.png)
```

### 视频

**方案 A：本地视频（小文件）**

将视频放入 `static/media/`，然后嵌入：

```html
<video controls src="/media/your-video.mp4" width="100%"></video>
```

**方案 B：外部视频（推荐，无大小限制）**

上传到 YouTube / Bilibili，然后嵌入 iframe：

```html
<iframe src="https://player.bilibili.com/player.html?bvid=BVxxxxxx" 
        width="100%" height="400" frameborder="0" 
        allowfullscreen></iframe>
```

### 音频

```html
<audio controls src="/media/your-audio.mp3"></audio>
```

> ⚠️ **GitHub 限制提醒**：
> - 单文件最大 **100MB**
> - 仓库总容量建议不超过 **1GB**
> - 视频文件通常很大，建议优先使用外部托管（YouTube、Bilibili）+ 嵌入

---

## 公开 vs 私密文章

Hugo 通过 `draft` 字段控制文章可见性：

| draft 值 | 效果 | 适用场景 |
|----------|------|----------|
| `false` | **公开发布** | 想分享的学习笔记 |
| `true` | **不发布**（源文件仍在 GitHub）| 私人草稿、未完成内容 |

示例：

```yaml
---
title: "私密笔记"
date: 2026-06-18T10:00:00+08:00
draft: true   # ← 这篇文章不会出现在网站上
tags: []
---
```

> **注意**：`draft: true` 只是不构建到网站中，源文件仍存在于 Git 仓库里。如果你需要**真正的加密私密**，建议：
> 1. 私人内容只保存在本地 Obsidian，不提交到 GitHub
> 2. 或创建一个**私有仓库**专门存放私密笔记

---

## 自定义域名（可选）

如果你不想用 `username.github.io`，可以购买自己的域名（约 ¥70/年）：

1. 购买域名（推荐 [Cloudflare](https://www.cloudflare.com/) 或 [Namecheap](https://www.namecheap.com/)）
2. 在域名服务商处添加 CNAME 记录，指向 `<your-username>.github.io`
3. 在项目根目录创建 `static/CNAME` 文件，内容为你的域名：
   ```
   yourdomain.com
   ```
4. 修改 `config.yml` 中的 `baseURL`
5. 推送更改

---

## 常见问题

### Q1: 网站没有更新？

1. 确认已成功 `git push`
2. 前往 GitHub 仓库 → **Actions** 标签，查看构建状态
3. 如果构建失败，点击工作流查看错误日志

### Q2: 如何修改网站外观？

编辑 `config.yml` 中的 `params` 部分，或参考 [PaperMod 文档](https://github.com/adityatelange/hugo-PaperMod/wiki)。

### Q3: 如何添加新菜单项？

在 `config.yml` 的 `menu.main` 部分添加：

```yaml
menu:
  main:
    - name: "新菜单"
      url: "/new-page/"
      weight: 6
```

然后创建对应页面 `content/new-page.md`。

### Q4: 本地预览网站？

如果你安装了 Hugo（技术用户），可以本地预览：

```bash
cd ~/my-knowledge-base
hugo server -D
# 访问 http://localhost:1313
```

非技术用户可以直接推送到 GitHub，通过 Actions 自动部署预览。

### Q5: 文章图片不显示？

确保图片放在 `static/media/` 目录下，引用路径以 `/media/` 开头：

```markdown
![描述](/media/image.png)  # ✅ 正确
![描述](media/image.png)   # ❌ 错误，缺少前导斜杠
```

---

## 备份与安全

- **Git 历史不可篡改**：每次提交都有唯一哈希，无法被悄悄修改
- **双重备份**：GitHub 远程仓库 + 本地仓库
- **免费**：除可选域名外，零费用

---

## 下一步

1. ✅ 阅读本 README
2. ✅ 修改 `config.yml` 中的个人信息
3. ✅ 注册 GitHub 并创建仓库
4. ✅ 推送项目到 GitHub
5. ✅ 启用 GitHub Pages
6. 📝 开始写作！

---

*构建日期：2026-06-18*  
*技术栈：Hugo v0.x + PaperMod + GitHub Pages*
