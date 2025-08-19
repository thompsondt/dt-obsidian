---
aliases:
  - "<% tp.date.now("MMMM[, ]YYYY", 0, tp.file.title, "YYYY-MM") %>"
  - "Monthly Note: <% tp.date.now("MMMM[, ]YYYY", 0, tp.file.title, "YYYY-MM") %>"
year: "[[Journal/<% tp.date.now("YYYY", 0, tp.file.title, "YYYY-MM") %>]]"
previous:
  - "[[Journal/<% tp.date.now("YYYY-MM", "P-1M", tp.file.title, "YYYY-MM") %>]]"
next:
  - "[[Journal/<% tp.date.now("YYYY-MM", "P1M", tp.file.title, "YYYY-MM") %>]]"
created: <% tp.file.creation_date() %>
tags:
  - monthly-note
---
<< [[Journal/<% tp.date.now("YYYY-MM", "P-1M", tp.file.title, "YYYY-MM") %>]] | (Year: [[Journal/<% tp.date.now("YYYY", 0, tp.file.title, "YYYY-MM") %>]]) (Quarter: [[Journal/<% tp.date.now("YYYY-[Q]Q", 0, tp.file.title, "YYYY-MM") %>]]) | [[Journal/<% tp.date.now("YYYY-MM", "P1M", tp.file.title, "YYYY-MM") %>]]  >>

# Monthly Note: <% tp.date.now("MMMM[, ]YYYY", 0, tp.file.title, "YYYY-MM") %>

Days:
<%*
for (let day = 0; day < moment(tp.file.title, "YYYY-MM").endOf("month").format("DD"); day++) {
	let date = tp.date.now("YYYY-MM-DD", day, tp.file.title, "YYYY-MM");
	tR += `- (days:: [[Journal/${date}|${date}]])\n`; //The root of the vault has an implied `/`
}
%>

(template::[[Monthly Note (Template)]])
