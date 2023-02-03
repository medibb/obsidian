

```dataview
table tags as "🌱️", file.ctime.year as CY, file.ctime.month as CM, file.ctime.day as CD, file.mtime.year as MY, file.mtime.month as MM, file.mtime.day as MD
from #🧠️/📝️/🌱️ 
where file.name != "Tag Taxonomy" AND file.name != "INDEX" AND file.name != "Notes"
sort file.ctime asc
```

```dataview
table tags as "🌿️", file.ctime.year as CY, file.ctime.month as CM, file.ctime.day as CD, file.mtime.year as MY, file.mtime.month as MM, file.mtime.day as MD
from #🧠️/📝️/🌿️ 
where file.name != "Tag Taxonomy" AND file.name != "INDEX" AND file.name != "Notes"
sort file.ctime asc
```

```dataview
table tags as "🌞️", file.ctime.year as CY, file.ctime.month as CM, file.ctime.day as CD, file.mtime.year as MY, file.mtime.month as MM, file.mtime.day as MD
from #🧠️/📝️/🌞️
where file.name != "Tag Taxonomy" AND file.name != "INDEX" AND file.name != "Notes" AND file.name != "Draft" AND file.name != "Presentation"
sort file.ctime asc
```

```dataview
table tags as "🌲️", file.ctime.year as CY, file.ctime.month as CM, file.ctime.day as CD, file.mtime.year as MY, file.mtime.month as MM, file.mtime.day as MD
from #🧠️/📝️/🌲️ 
where file.name != "Tag Taxonomy" AND file.name != "INDEX" AND file.name != "Notes"
sort file.ctime asc
```
