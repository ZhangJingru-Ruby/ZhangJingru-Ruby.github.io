---
layout: post
title: "How to Add a New Tab Section to My Website (Like 'rl' or 'worklog')"
date: 2025-06-08
category: [coding]
image: 20250608.jpg
description: A personal guide on how to add a new tag-based section to my site, complete with a preview block and tag archive. Think 'rl', 'coding', 'teaching'... 🌟
---

If I want to create a new section (like **RL**, **Worklog**, **Teaching**, etc.) that shows up under the **Work** or **Notes** tabs, here's my full ritual 🧙‍♀️✨

---

## 🧱 Step 1: Write Your Posts with the Right Tag

When creating a post (in `_posts/`), use a tag to define which section it belongs to.

Example front matter:

```yaml
---
layout: post
title: "Understanding Actor-Critic Algorithms"
date: 2025-06-08
tags: [rl]
image: rl-cover.jpg
description: My notes on A2C vs PPO, with visual metaphors and intuition dumps 🧠
---
```

---

## ✨ Step 2: Add a Preview Block to the Work or Notes Page

Inside `work.md` or `notes.md`, add a section like this:

```liquid
<!-- RL Section -->
<div class="work-block">
  <h3>RL</h3>
  <p>Study notes and diagrams for reinforcement learning concepts 📘</p>
  {% include section-preview.html tag="rl" limit="3" %}
  <a href="{{ site.baseurl }}/tags/rl" class="button">More →</a>
</div>
```

Replace:
- `rl` with your new tag
- the paragraph with a cute description
- the emoji 😘 with a cuter one

---

## 🗂️ Step 3: Create a Tag Archive Page

Inside `_tags/`, create a file called (for example) `rl.md`:

```markdown
---
layout: tag_page
title: Reinforcement Learning
tag: rl
permalink: /tags/rl/
---
```

> 📝 Use the same `tag:` name as in the post’s front matter!

Repeat this for each tag-based section you want to create:  
`coding.md`, `teaching.md`, `worklog.md`, etc.

---

## 🛠️ Step 4: Commit & Push

```bash
git add _posts/2025-06-09-add-tag-section.md _tags/rl.md
git commit -m "🧩 Add post about creating new tag-based sections like 'rl'"
git push origin main
```

Boom. The new section is live! It’ll appear inside the tab page (like Notes or Work), and the “More →” button will lead to a full archive page of all posts with that tag. 🥰

---

## 💡 Bonus Ideas

- Want to style the tag page layout? Edit `_layouts/tag_page.html`
- Want to sort by date or title? Add sorting logic in `section-preview.html`

