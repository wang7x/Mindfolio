---
type: daily note
created: <% tp.file.creation_date() %>
template: Daily Notes Templates V1.1
---
tags:: [[+Daily Notes]]

---
## 📋 Tasks

#### ☑️ Todo today
```tasks
not done
```

#### ✅ Tasks done today
```tasks
done on <%tp.date.now("YYYY-MM-DD")%> sort by done
```

#### 📋New tasks today

---
## ⏳Timeline
- 🏷️ Activity Type Abbr: DW(Deep Work:focused/uninterrupted), CW(Collab Work:meetings/communication), DD(Daily Duties:email/IM/Small Tasks), LG(Learning & Growth), MF(Movement & Fitness), RM(Reading & Meditation), LE(Leisure)
- ⚡ State: 1- Extremely fatigued (unfocused), 2- Barely functional, 3- Steady work mode, 4- Highly productive flow, 5- Exceptional creativity  
- 🎯 Productivity: 1-Severe delay/no output (<20%), 2-Slow progress (20%-40%), 3-Average pace (40%-60%), 4-High efficiency (60%-80%), 5-Flow state (>80%)  

|    🕒 Time    | 📝 Activity | 🏷️ Type | ⚡ State | 🎯 Prod. | 📝 Notes |
| :---------: | :----- | :-----: | :-: | :--: | :--: |
| 00:00-06:00 |        |         |     |      |      |
| 06:00-08:00 |        |         |     |      |      |
| 09:00-10:00 |        |         |     |      |      |
| 10:00-11:00 |        |         |     |      |      |
| 11:00-12:00 |        |         |     |      |      |
| 12:00-14:00 |        |         |     |      |      |
| 14:00-15:00 |        |         |     |      |      |
| 15:00-16:00 |        |         |     |      |      |
| 16:00-17:00 |        |         |     |      |      |
| 17:00-18:00 |        |         |     |      |      |
| 18:00-19:00 |        |         |     |      |      |
| 19:00-20:00 |        |         |     |      |      |
| 20:00-22:00 |        |         |     |      |      |
| 22:00-24:00 |        |         |     |      |      |
```meta-bind-button
label: New Meeting
hidden: false
class: ""
tooltip: ""
id: ""
style: default
actions:
  - type: templaterCreateNote
    templateFile: Templates/Meeting Template.md
    folderPath: Timestamps/Meetings
    fileName: TKTK
    openNote: true
```
---
## 📝 Notes

 <% tp.file.cursor() %>

---
## 📅 Daily Questions

##### 💪Today's top achievement or happiest moment?  
-  

##### 🙌Key challenge faced? What did I learn?
-  

##### 🌱What could be improved? Concrete steps? 
*(or: What specific change would I make if I could relive today? and why?)*
- 

##### 😊What am I most grateful for today?
-  

##### 🚀Tomorrow's top priority
-  

---
## 🌄 Daily Vision


---
### Notes created today
```dataview
List FROM "" WHERE file.cday = date("<%tp.date.now("YYYY-MM-DD")%>") SORT file.ctime asc
```

### Notes last touched today
```dataview
List FROM "" WHERE file.mday = date("<%tp.date.now("YYYY-MM-DD")%>") SORT file.mtime asc
```