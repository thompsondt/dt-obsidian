---
aliases:
  - "<% tp.date.now("gggg [Week] ww", 0, tp.file.title, "gggg-[W]ww") %>"
month: "[[Journal/<% tp.date.now("gggg-MM", 0, tp.file.title, "gggg-[W]ww") %>]]"
previous:
  - "[[Journal/<% tp.date.now("gggg-[W]ww", -1, tp.file.title, "gggg-[W]ww") %>]]"
next:
  - "[[Journal/<% tp.date.now("gggg-[W]ww", 7, tp.file.title, "gggg-[W]ww") %>]]"
created: <% tp.file.creation_date() %>
tags:
  - weekly-note
template: "[[Weekly Note (Template)]]"
---
<< [[Journal/<% tp.date.now("gggg-[W]ww", -1, tp.file.title, "gggg-[W]ww") %>]] | (Month: [[Journal/<% tp.date.now("gggg-MM", 0, tp.file.title, "gggg-[W]ww") %>]]) | [[Journal/<% tp.date.now("gggg-[W]ww", 7, tp.file.title, "gggg-[W]ww") %>]]  >>
# <% tp.date.now("gggg [Week] ww", 0, tp.file.title, "gggg-[W]ww") %>

> [!NOTE]- Zoom Out (Monthly View) 
> ![[Journal/<% tp.date.now("gggg-MM", 0, tp.file.title, "gggg-[W]ww") %>#Objectives]]

## This Week

- [[Journal/<% tp.date.now("YYYY-MM-DD", 0, tp.file.title, "gggg-[W]ww") %>|<% tp.date.now("dddd[, ]MMMM Do", 0, tp.file.title, "gggg-[W]ww") %>]]
- [[Journal/<% tp.date.now("YYYY-MM-DD", 1, tp.file.title, "gggg-[W]ww") %>|<% tp.date.now("dddd[, ]MMMM Do", 1, tp.file.title, "gggg-[W]ww") %>]]
- [[Journal/<% tp.date.now("YYYY-MM-DD", 2, tp.file.title, "gggg-[W]ww") %>|<% tp.date.now("dddd[, ]MMMM Do", 2, tp.file.title, "gggg-[W]ww") %>]]
- [[Journal/<% tp.date.now("YYYY-MM-DD", 3, tp.file.title, "gggg-[W]ww") %>|<% tp.date.now("dddd[, ]MMMM Do", 3, tp.file.title, "gggg-[W]ww") %>]]
- [[Journal/<% tp.date.now("YYYY-MM-DD", 4, tp.file.title, "gggg-[W]ww") %>|<% tp.date.now("dddd[, ]MMMM Do", 4, tp.file.title, "gggg-[W]ww") %>]]
- [[Journal/<% tp.date.now("YYYY-MM-DD", 5, tp.file.title, "gggg-[W]ww") %>|<% tp.date.now("dddd[, ]MMMM Do", 5, tp.file.title, "gggg-[W]ww") %>]]
- [[Journal/<% tp.date.now("YYYY-MM-DD", 6, tp.file.title, "gggg-[W]ww") %>|<% tp.date.now("dddd[, ]MMMM Do", 6, tp.file.title, "gggg-[W]ww") %>]]
