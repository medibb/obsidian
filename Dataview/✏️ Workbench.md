
```dataview
TABLE dateformat(file.mtime, "dd.MM.yyyy - HH:mm") AS "Last modified"
FROM -"Utility" AND -"Dataview" AND -"Template" AND !"Z"
SORT file.mtime DESC
LIMIT 10
where problems = dep
```

