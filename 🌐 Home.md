## MOCs
```dataview
LIST
FROM #MOC
SORT file.name ASC
```

## Daily Notes & Meetings

```dataview
TABLE
    type AS "Type",
    created AS "Created"
FROM "Timestamps"
SORT
    created DESC
LIMIT 10
```

## Notes last touched

```dataview
List FROM "" 
SORT file.mtime DESC
LIMIT 20
```