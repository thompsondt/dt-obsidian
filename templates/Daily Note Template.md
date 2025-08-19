---
aliases:
  - "<% tp.date.now("dddd[, ]MMMM Do[, ]YYYY", 0, tp.file.title, "YYYY-MM-DD") %>"
  - "Daily Note: <% tp.date.now("dddd[, ]MMMM Do[, ]YYYY", 0, tp.file.title, "YYYY-MM-DD") %>"
month: "[[Journal/<% tp.date.now("YYYY-MM", 0, tp.file.title, "YYYY-MM-DD") %>]]"
week: "[[Journal/<% tp.date.now("gggg-[W]ww", 0, tp.file.title, "YYYY-MM-DD") %>]]"
created: <% tp.date.now("YYYY-MM-DDTHH:mm:ss") %>
previous:
  - "[[<% tp.date.now("YYYY-MM-DD", -1, tp.file.title, "YYYY-MM-DD") %>]]"
next:
  - "[[<% tp.date.now("YYYY-MM-DD", +1, tp.file.title, "YYYY-MM-DD") %>]]"
tags:
  - daily-note
---
<< [[Journal/<% tp.date.now("YYYY-MM-DD", -1, tp.file.title, "YYYY-MM-DD") %>]] | (Month: [[Journal/<% tp.date.now("YYYY-MM", 0, tp.file.title, "YYYY-MM-DD") %>]]) (Week: [[Journal/<% tp.date.now("gggg-[W]ww", 0, tp.file.title, "YYYY-MM-DD") %>]]) | [[Journal/<% tp.date.now("YYYY-MM-DD", +1, tp.file.title, "YYYY-MM-DD") %>]]  >>
# Daily Note: <% tp.date.now("dddd[, ]MMMM Do[, ]YYYY", 0, tp.file.title, "YYYY-MM-DD") %>

> [!NOTE]- Zoom Out (Monthly View) 
> ![[Journal/<% tp.date.now("YYYY-MM", 0, tp.file.title, "YYYY-MM-DD") %>#Objectives]]

## Other Notes

> [!TIP]- Dataview
> ```dataview
> list
> where
> 	!contains(file.tags, "daily-note") and
> 	contains(file.outlinks, this.file.link) or
> 	contains(string(file.frontmatter), string(dateformat(this.file.day,"yyyy-MM-dd")))
> sort file.ctime asc
> limit 50
> ```
