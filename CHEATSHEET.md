# Website Cheat Sheet

## Quick Start

```bash
cd /d D:\Obsidian\yiwen\Website\blog
C:\Users\Administrator\bin\hugo.exe server
```
Then open http://localhost:1313 to preview.

---

## Write a New Post

1. Create a file in `content\posts\` — name it with dashes, e.g. `my-new-post.md`
2. Use this template:

```markdown
---
title: "Your Post Title"
date: 2026-04-04
draft: false
---

Your content here in Markdown.

## Subheading

- bullet point
- **bold text**
- *italic text*

> blockquote

[link text](https://example.com)
```

3. Preview at http://localhost:1313
4. Publish (see below)

---

## Publish Changes

```bash
cd /d D:\Obsidian\yiwen\Website\blog
git add -A
git commit -m "Add new post: your title"
git push origin main
```

Site auto-deploys to https://tuoyiwen.github.io in ~1 minute.

---

## Common Tasks

| Task | How |
|------|-----|
| **Edit bio** | Change `bio` in `hugo.toml` |
| **Update photo** | Replace `static\img\download.jpg` |
| **Edit social links** | Change `[params.social]` in `hugo.toml` |
| **Hide a draft** | Set `draft: true` in post frontmatter |
| **Preview drafts** | `hugo.exe server --buildDrafts` |
| **Change site title** | Change `title` in `hugo.toml` |

---

## File Structure

```
blog\
  content\posts\       ← your blog posts (Markdown)
  content\archive\     ← archive page
  static\img\          ← images (avatar, etc.)
  static\css\style.css ← site styling
  layouts\             ← HTML templates
  hugo.toml            ← site config (title, bio, links)
```

---

## Markdown Quick Reference

```markdown
**bold**        *italic*        ~~strikethrough~~
# H1           ## H2           ### H3
- bullet       1. numbered     > blockquote
[link](url)    ![image](path)
`inline code`  ```code block```
| col | col |  ← tables
```
