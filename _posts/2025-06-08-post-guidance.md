---
layout: post
title: "How to Add a New Post to My Website"
date: 2025-06-08
tags: [coding]
image: 20250608-2.jpg
description: A step-by-step guide I wrote for myself (and future me!) on how to write, style, and publish a new post on my GitHub-powered site 💻✨
---

## 🪄 Step 1: Create Your New Markdown File

In your project folder, navigate to:

```
_pages/      ← for pages like About, Notes, etc.  
_posts/      ← for blog-style content (like this!)
```

Inside `_posts/`, create a new file. The filename must follow this pattern:

```
YYYY-MM-DD-title-of-your-post.md
```

Example:
```
2025-06-09-how-to-add-post.md
```

---

## 📝 Step 2: Add the Standard Front Matter

At the top of your post file, paste this (and adjust it!):

```yaml
---
layout: post
title: "Your Post Title Here"
date: 2025-06-08
tags: [worklog, rl, teaching]  # use one or more existing tags
image: 01.jpg                  # optional — image must be in /images/
description: A short one-sentence teaser for preview cards.
---
```

> 🐣 If you're not using an image, just remove the `image:` line.

---

## ✍️ Step 3: Write Your Content

Use **Markdown syntax** as usual.

---

## 🌸 Step 4: Commit & Push to GitHub

Open Git Bash and run:

```bash
git add _posts/2025-06-09-how-to-add-post.md images/new_image.jpg
git commit -m "📝 Add guide for writing and publishing a new post"
git push origin main
```

Your post will appear automatically under the corresponding section in `/work/`, `/notes/`, or the tag archives!

---

## 🌟 Bonus Tips

- Keep image files in `/images/`
- Use `description:` for prettier previews
- Use one of your existing tags like `rl`, `coding`, `teaching`, `worklog`, `projects`, etc
- Preview locally with:
  ```bash
  bundle exec jekyll serve
  ```

