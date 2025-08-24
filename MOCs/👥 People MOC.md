[[🌐 Home]] #MOC

```meta-bind-button
label: New People Note
hidden: false
class: ""
tooltip: ""
id: ""
style: primary
actions:
  - type: templaterCreateNote
    templateFile: Templates/People Template.md
    folderPath: People
    fileName: Enter Name Here
    openNote: true

```

# People MOC
A personal CRM. People Notes are about jotting down notable information about people and linking people back to [[🗣 Meetings MOC]].

These are the different categories of People Notes:
- Work
- Personal
- Fictional
- Notable

---
### Templates
- [[People Template]]

# People
```dataview
table title
from "People"
sort file.name asc
```
