<div align="center">

**A minimal, directory-style Jekyll blog theme.**

[![Jekyll](https://img.shields.io/badge/Jekyll-4.x-red?style=flat-square&logo=jekyll)](https://jekyllrb.com)
[![License](https://img.shields.io/badge/License-MIT-black?style=flat-square)](LICENSE)
[![Based on](https://img.shields.io/badge/Based%20on-Elementary-555?style=flat-square)](https://github.com/abhn/Elementary)
[![Made by](https://img.shields.io/badge/Made%20by-0xrwise-111?style=flat-square)](https://github.com/0xrwise)

<br/>

*Research, Reflect, Wisdom.*

</div>

---

## / what is this

**0xdir** is a Jekyll blog theme built on top of [Elementary](https://github.com/abhn/Elementary) by [@abhn](https://github.com/abhn), redesigned from the ground up with a directory-listing aesthetic — inspired by the raw, no-nonsense look of `Index of /` pages you find on FTP servers and file mirrors.

No bloat. No unnecessary frameworks. Just your words, clean typography, and a theme that gets out of the way.

---

## / preview

```
Home | Tags | About | RSS                              [ Dark ]
─────────────────────────────────────────────────────────────
My Blog
/ index of posts
─────────────────────────────────────────────────────────────
▶  NEWS                                            2 entries
▼  ESSAYS                                          4 entries
│
│  01/2024    On Writing Simply
│  01/2024    The Beauty of Plain Text
│  12/2023    Why I Switched to Jekyll
│  11/2023    Building in Public
│
─────────────────────────────────────────────────────────────
```

> Supports **light mode**, **dark mode**, and **auto mode** (follows your OS).

---

## / features

```
✦  Directory-style post listing     clean, scannable, minimal
✦  Auto dark / light mode           follows OS preference
✦  Manual toggle                    saved to cookie
✦  No flash on load                 theme applied before render
✦  Monospace + Serif typography     Geist Mono + Source Serif 4
✦  Collapsible post categories      smooth expand/collapse
✦  Scroll progress bar              top of post pages
✦  Tag system                       filter posts by topic
✦  Featured posts                   shown at bottom of articles
✦  RSS feed                         built-in via jekyll-feed
✦  Zero JS dependencies             vanilla JS only
✦  Mobile friendly                  responsive layout
✦  Fast                             static HTML, no bloat
```

---

## / quick start

**Requirements:** Ruby 3.x, Bundler

```bash
# 1. Use this template (click "Use this template" button above)
#    or clone directly:
git clone https://github.com/0xrwise/0xdir.git my-blog
cd my-blog

# 2. Install dependencies
bundle install

# 3. Run locally
bundle exec jekyll serve

# 4. Open in browser
# → http://localhost:4000
```

---

## / structure

```
0xdir/
│
├── _config.yml          ← site settings
├── index.html           ← homepage
├── tags.html            ← tags index
├── about.md             ← about page
│
├── _layouts/
│   ├── default.html     ← base layout
│   ├── page.html        ← static pages
│   └── post.html        ← blog posts
│
├── _includes/
│   ├── head.html        ← <head> + fonts + dark mode init
│   ├── nav.html         ← top navigation
│   └── featured.html    ← featured posts block
│
├── assets/
│   ├── main.css         ← all styles (single file, no SASS needed)
│   └── main.js          ← dark mode toggle + scroll progress
│
├── _essays/             ← write your essays here
└── _news/               ← write your news/updates here
```

---

## / writing posts

Create a `.md` file in `_essays/` or `_news/`:

```markdown
---
title: "Your Post Title"
date: 2026-01-01
tags: [writing, thoughts]
---

Your content here. **Markdown** supported.
```

File name format: `YYYY-MM-DD-post-slug.md`

---

## / configuration

Edit `_config.yml` to make it yours:

```yaml
title: "Your Blog"
name:  "Your Blog"
description: "What your blog is about"
url: "https://yourusername.github.io"

author:
  name: "Your Name"

javascript_enabled: true          # show dark/light toggle
featured_posts_title: "Featured"  # label for featured section

featured_posts:                   # posts to feature at bottom of articles
  - url: /essays/your-post
    title: Your Post Title
```

---

## / deploy to GitHub Pages

```bash
# 1. Create a repo on GitHub named:
#    yourusername.github.io  (for user site)
#    or any name            (for project site)

# 2. Push your code
git init
git add .
git commit -m "init: 0xdir blog"
git remote add origin https://github.com/USERNAME/REPO.git
git branch -M main
git push -u origin main

# 3. Go to repo Settings → Pages → Source: main branch
# 4. Your site is live at https://USERNAME.github.io
```

---

## / credits & license

**0xdir** is built on top of [Elementary](https://github.com/abhn/Elementary) by [Nagekar Abhishek](https://github.com/abhn), which is licensed under GPL-3.0.

Custom design, CSS rewrite, dark mode system, and all modifications by **M. Rafi Akbar** ([@0xrwise](https://github.com/0xrwise)) — released under the [MIT License](LICENSE).

```
Copyright (c) 2026 M. Rafi Akbar (0xrwise)
```

---

<div align="center">

made with ♥ and a terminal

**[⭐ star this repo if you like it](https://github.com/0xrwise/0xdir)**

</div>
