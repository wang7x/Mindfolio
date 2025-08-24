---
type: People
category:  Work | Personal | Fictional | Notable
phone: +86
wechat:
email:
company:
title:
employeeId:
location:
birthday:
website:
aliases:
template: People Template V1.1
---
tags:: [[👥 People MOC]]

# [[<% tp.file.title %>]]
<% await tp.file.move("/People/" + tp.file.title) %>

## Notes
-

## Characteristics

> *Documenting traits helps us understand each other better, and learning preferences enables smoother communication. Keep these principles in mind:
>   - **Avoid fixed labels**: People grow and change over time. Outward behaviors don't reflect unchangeable truths
>   - **Respect differences**: The goal is better collaboration, not judgment
>   - **Begin with good intentions**: Draw inspiration from others' strengths and experiences to build cooperation and mutual understanding
> *Reference: OCEAN (Big Five) personality traits model*

##### **O**penness (Inventive/Curious vs. Consistent/Cautious)
-

##### **C**onscientiousness (Efficient/Organized vs. Easygoing/Careless)
-

##### **E**xtraversion (Outgoing/Energetic vs. Solitary/Reserved)
-

##### **A**greeableness (Compassionate/Cooperative vs. Critical/Detached)
-

##### **N**euroticism (Sensitive/Anxious vs. Resilient/Confident)
-

## Meetings
```dataview
TABLE file.cday as Created, summary AS "Summary"
FROM "Timestamps/Meetings" where contains(file.outlinks, [[]])
SORT file.cday DESC
```
