---
tags:
  - map-of-content
indexes (MOCs):
  - "[[MOC INBOX (MOC)]]"
---
> [!WARNING] Do Not Change These Special Headings
> - `%%Export: Index+Title%%` -- supports cleanly embedding the MOCs content without breaking when the title changes.

###### %%Export: Index+Title%%

**`= [[]].title`** %% Don't Edit this line. Place list items below this bullet point. %%


## Index Requests

These items have linked here in their YAML data with `indexes (MOCs): filename`, but are into in the index.
```dataview
LIST
FROM [[]]
WHERE contains(indexes-mocs, [[]])
WHERE !contains(file.inlinks, [[]])
LIMIT 10
```
