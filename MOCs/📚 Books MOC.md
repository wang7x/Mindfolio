---
aliases: ["📚 Books"]
---
[[🌐 Home]] #MOC

```meta-bind-button
label: New Book
hidden: false
class: ""
tooltip: ""
id: ""
style: default
actions:
  - type: templaterCreateNote
    templateFile: Templates/Books Template.md
    folderPath: Books
    fileName: Book Name
    openNote: true

```

# Template
- [[Books Template]]

# Books
```dataview
TABLE Date, Title, Author
FROM "Books"
SORT file.name DESC
```
