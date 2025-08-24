---
aliases: ["🧭 PARA MOC"]
---
[[🌐 Home]] #MOC

# PARA MOC
## 📂 Projects

```meta-bind-button
label: New Project
hidden: false
class: ""
tooltip: ""
id: ""
style: default
actions:
  - type: templaterCreateNote
    templateFile: Templates/Project Template.md
    folderPath: Projects
    fileName: Project Name
    openNote: true
```

```dataview
TABLE
    status AS "Status",
    priority AS "Priority",
    created AS "Created",
    due AS "Due"
FROM "Projects"
WHERE type = "project"
  AND (status = "active" OR status = "paused")
SORT
    priority DESC,
    due ASC
```

### Completed Projects
```dataview
TABLE
    priority AS "Priority",
    created AS "Created",
    due AS "Due"
FROM "Projects"
WHERE type = "project"
  AND status = "completed"
SORT
    due DESC
LIMIT 5
```

## 🛠️ Areas

```meta-bind-button
label: New Area
hidden: false
class: ""
tooltip: ""
id: ""
style: default
actions:
  - type: templaterCreateNote
    templateFile: Templates/Area Template.md
    folderPath: Areas
    fileName: Area Name
    openNote: true
```

```dataview
TABLE
    review AS "Review",
    created AS "Created"
FROM "Areas"
WHERE type = "area"
SORT
    created DESC
LIMIT 10
```

## 📚 Resources

```meta-bind-button
label: New Resource
hidden: false
class: ""
tooltip: ""
id: ""
style: default
actions:
  - type: templaterCreateNote
    templateFile: Templates/Resource Template.md
    folderPath: Resources
    fileName: Resource Name
    openNote: true
```

```dataview
TABLE
    link(file.name) AS "Resource",
    category AS "Category",
    created AS "Created"
FROM "Resources"
WHERE type = "resource"
SORT
    created DESC
LIMIT 10
```

## 📦 Archives(Latest 10)

```dataview
TABLE
    type AS "Type",
    created AS "Created"
FROM "Archives"
SORT
    created DESC
LIMIT 10
```