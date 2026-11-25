# Writing a blog post

1. Copy `_drafts/post-template.md` to `_posts/YYYY-MM-DD-short-title.md`
   (for example `_posts/2026-12-01-flow-matching-vla.md`). The date in the filename is the publish date.
2. Put any images in `assets/img/blog/<short-title>/` and reference them as
   `![alt text](/assets/img/blog/<short-title>/figure.png)`.
3. Commit and push to `main`. GitHub Actions rebuilds the site and the post appears under **Blogs** in a few minutes.

## Front matter

```yaml
---
title: "Your Post Title"
date: 2026-12-01
description: "One or two sentences shown on the Blogs page."
tags: [world-models, rl]
# toc: {beginning: false}   # optional: hide the table of contents
# citation: false           # optional: hide the Citation block
---
```

Layout, author, table of contents, and the citation block are set by default in `_config.yml`, so you don't need to add them.

## Math

- Inline: `$a^2 + b^2 = c^2$`
- Display: put `$$ ... $$` on its own lines, with a blank line before and after.
- Use `\begin{align} ... \end{align}` inside `$$` for numbered multi-line equations, with `\label{}` and `\eqref{}`.
- Markdown runs before MathJax. If an inline formula with `*` or `\\` renders oddly, write it with `$$ ... $$` inside the sentence instead (kramdown treats inline `$$x$$` as inline math).

## Previewing locally

```bash
bundle exec jekyll serve --drafts
```

Then open http://localhost:4000/blog/. Files in `_drafts/` only show up with `--drafts`, so they never appear on the live site.
