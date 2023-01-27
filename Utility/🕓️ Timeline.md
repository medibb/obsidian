  
## Unprocessed / WIP

```dataview
list 
from "Z" OR "Inbox" AND !"Journal" AND !"Templates"
where file.day = null AND type != null
sort file.day desc
```

## Processed

```dataview
list
from "Z" OR "Inbox" AND !"Journal" AND !"Templates"
where type != null AND file.day
sort file.day desc
```

LINKS TO THIS PAGE

[[INDEX]]