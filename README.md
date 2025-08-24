# Obsidian Knowledge Base Template

This repository contains a template for structuring a personal knowledge base in [Obsidian](https://obsidian.md/). It's inspired by [Dan Berg's Gist](https://gist.github.com/dannberg) and aims to provide a simple yet effective way to organize notes.

## 🧠 Mindfolio: A PARA-Driven Knowledge System in Obsidian

### Overview

Welcome to **Mindfolio**, a modular, reproducible, and extensible knowledge management system built in Obsidian. This vault is designed to serve as a cockpit-style dashboard for your mind — combining the strategic clarity of PARA with the automation power of Advanced Tables, Dataview, Meta Bind, Tasks, Templater.

---

## 🧩 Philosophy

**Name Interpretation: Mindfolio**

**Mindfolio = Mind + Portfolio**

- **Mind**: Represents cognition, insight, learning, and creativity. It reflects the way you manage knowledge and hints at the depth of thought behind your information architecture.
- **Portfolio**: More than just a showcase of work — it’s a strategic container. It implies the asset-based management of knowledge, where each note is an investment and each project is a pool of intellectual capital.

**Metaphorical Layer**:

- Mindfolio is the “balance sheet” of your mind, tracking how you accumulate, allocate, and optimize cognitive resources.
- It is also a “cognitive cockpit,” where PARA, Dataview, and Templater transform abstract thinking into a visual, actionable system.

Mindfolio is not just a note-taking system — it's a cognitive operating system. It transforms scattered thoughts into structured assets, enabling you to think in systems, act with clarity, and iterate with precision.

---

## 🚀 Getting Started

1. **Install Obsidian**: Download from [obsidian.md](https://obsidian.md)
2. **Clone/copy this vault structure**:

```bash
git clone https://github.com/wang7x/mindfolio.git
```

3. **Enable Community Plugins**:

- Open Obsidian Settings → Community plugins
- Install the following plugins:
  - [Advanced Tables Obsidian](https://github.com/tgrosinger/advanced-tables-obsidian)
  - [Dataview](https://github.com/blacksmithgu/obsidian-dataview)
  - [Meta Bind](https://github.com/mProjectsCode/obsidian-meta-bind-plugin)
  - [Tasks](https://github.com/obsidian-tasks-group/obsidian-tasks)
  - [Templater](https://github.com/SilentVoid13/Templater)
- Enable these plugins in Obsidian settings.

4. **Set Core Plugins**:

- Set `Core Plugins - Templates` template folder location to `Templates/` in vault settings
- Set `Core Plugins - Daily Notes` Configuration

  ```
  {
    "template": "Templates/Daily Note Template",
    "folder": "Timestamps",
    "format": "YYYY/YYYY-MM/YYYY-MM-DD-dddd",
    "autorun": false
  }
  ```

5. Explore dashboards in `/Home.md` for centralized control.
___

## 💡 USAGE

### 🌐 Home Dashboard
Your central control panel containing:
- Quick access to all MOCs (Maps of Content)
- System status overview
- Recent activity feed

### Core MOCs Navigation:

#### 🧭 PARA MOC
Your productivity engine using the PARA methodology:
1. **Projects**: Active initiatives with deadlines
   - Use "New Project" button → [[Project Template]]
   - Track status/priority in dataview tables
2. **Areas**: Ongoing responsibilities
   - Create with "New Area" button → [[Area Template]]
3. **Resources**: Reference materials
   - Add via "New Resource" button → [[Resource Template]]
4. **Archives**: Completed items storage

#### 👥 People MOC
Your personal CRM:
- Track relationships with "New People Note" button → [[People Template]]
- Categorize contacts (Work/Personal/Creative)

#### 📚 Books MOC
Knowledge repository:
- Add books with "New Book" button → [[Books Template]]
- Automatic sorting by date/author
- Track reading progress and key insights

#### 🗣 Meetings MOC
Conversation management:
- Create timestamped meetings → [[Meeting Template]]
- Ephemeral notes automatically archived
- Extract evergreen notes to appropriate MOCs

### 📅 Daily Notes System
Your operational cockpit for daily work:
1. **Automatic Creation**:
   - New daily notes auto-generate using [[Daily Note Template]]
   - Contains time-blocking table and reflection prompts

2. **Core Components**:
   - **Task Tracking**:
     - `☑️ Todo today`: Pending tasks from Tasks plugin
     - `✅ Tasks done today`: Automatically shows completed tasks
   - **Timeline Tracking**:
     ```md
     | 🕒 Time  | 📝 Activity | 🏷️ Type | ⚡ State | 🎯 Prod. | 📝 Notes |
     |----------|------------|---------|---------|---------|---------|
     ```
     - **Activity Types**:
       - DW (Deep Work), CW (Collaboration Work)
       - DD (Daily Duties), LG (Learning & Growth)
       - MF (Movement & Fitness), RM (Reading/Meditation)
     - **State Scale**: 1 (Fatigued) → 5 (Creative Flow)
     - **Productivity Scale**: 1 (<20% output) → 5 (>80%)
   - **Meeting Integration**:
     - Use "New Meeting" button → [[Meeting Template]]

3. **Daily Reflection**:
   - Answer core questions to improve productivity:
     - Today's achievement 💪
     - Key challenge & lesson 🙌
     - Improvement steps 🌱
     - Gratitude 😊
     - Tomorrow's priority 🚀

4. **Automatic Tracking**:
   - `Notes created today`: Dataview list of daily creations
   - `Notes last touched today`: Shows modified notes

---

## 📬 Feedback & Iteration

This system is designed for continuous improvement. Feel free to fork, remix, or contribute ideas. Every tweak is a step toward a more powerful mind.

## License

This project is licensed under the [MIT License](./LICENSE).
