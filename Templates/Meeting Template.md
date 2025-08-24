---
created: <% tp.file.creation_date("YYYY-MM-DD") %>
type: meeting
company: 
summary: 
template: Meeting Template V1.1
---
tags: [[🗣 Meetings MOC]]
Date:  [[<% tp.date.now("YYYY-MM-DD-dddd") %>]]
Begin Time:  <% tp.date.now("HH:mm") %>
End Time: <% tp.date.now("HH:mm") %>
<% await tp.file.rename(tp.date.now("YYYY-MM-DD") + " " + tp.file.title) %>
# [[<% tp.date.now("YYYY-MM-DD") + " " + tp.file.title %>]]

**Attendees**: 
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
- 

## Agenda/Questions
- 

## Notes
-

## Action Items
*List unresolved tasks and responsibilities from the meeting*

| Item | Owner | Deadline |
| ---- | ----- | -------- |
|      |       |          |
