# 🚀 Project Launch Tracker

A powerful, zero-dependency project tracking app that runs entirely in the browser. No server, no database, no login required — just open and start tracking.

![Project Launch Tracker](https://img.shields.io/badge/status-active-brightgreen) ![License](https://img.shields.io/badge/license-MIT-blue) ![Dependencies](https://img.shields.io/badge/dependencies-0-green)

## ✨ Features

### 📋 Project Planning
- **AI-Assisted Plan Builder** — Describe your project in natural language and get a full plan with smart durations, risk analysis, and recommendations
- **Import from anywhere** — Excel (.xlsx), CSV, JSON, or paste from Google Sheets
- **Manual creation** — Build milestone by milestone with full control

### 🤖 AI Project Assistant
- Natural language commands to update your project: *"Rebase all dates to 2026"*, *"Assign all unassigned to Sarah"*, *"Add 3 testing milestones"*
- Context-aware quick actions based on your project's current state
- Smart date detection and rebasing for imported plans

### 📅 Multiple Views
| View | Description |
|------|-------------|
| **Dashboard** | Health indicator, progress bar, key stats, milestone overview |
| **Timeline** | Gantt-style chart with phase grouping, today marker, color-coded bars |
| **Milestones** | Cards, Table, Kanban (drag & drop), or Calendar view |
| **People** | Per-person workload breakdown, completion rates, activity |
| **Documents** | Attach Google Docs, Sheets, Slides, Figma, GitHub, any URL |
| **Activity** | Full audit log with filters by change type and person |
| **Slides** | Auto-generated presentation with full-screen mode |

### 🎯 Project Management
- **Status tracking** — Not Started, In Progress, At Risk, Blocked, Complete
- **Inline editing** — Click any field to edit directly on cards or table rows
- **Bulk actions** — Select multiple milestones → change status, owner, phase, dates
- **Date rebasing** — Rebase to year, shift by days, or start from a specific date
- **Comments** — Add comments to any milestone with timestamps
- **Blank owners** — Create milestones without owners and assign later

### 🔗 Sharing
- **Shareable links** — Generate a URL that embeds your entire project data
- **JSON export/import** — Full project backup and restore
- **No server required** — Everything runs client-side

## 🚀 Quick Start

### Option 1: Open directly
Just open `index.html` in your browser. That's it!

### Option 2: Deploy to any static host
Upload `index.html` to GitHub Pages, Netlify, Vercel, or any static file host.

### Option 3: Share a project
1. Open the app and set up your project
2. Click **🔗 Share** in the top bar
3. Copy the generated link
4. Anyone who opens it will see your project pre-loaded

## 📖 Usage

### Creating a Project

**AI-Assisted:**
```
Describe: "We're building a customer portal with SSO, dashboard analytics, 
and API integrations. Timeline is 4 months with a team of 5. SOC2 compliant."
```
The AI analyzes your description and generates milestones with smart durations, dependencies, risk flags, and recommendations.

**Import:** Upload an Excel file or paste from Google Sheets. The app auto-detects column headers and maps them to milestone fields.

**Manual:** Click "+ Milestone" and fill in the details.

### AI Assistant Commands

| Command | What it does |
|---------|-------------|
| `Rebase all dates to 2026` | Moves all dates to target year |
| `Shift all dates forward 2 weeks` | Shifts every date by N days/weeks/months |
| `Start plan from today` | Rebases so earliest milestone starts today |
| `Mark all planning milestones as complete` | Bulk status change by phase |
| `Assign all unassigned to John` | Bulk owner assignment |
| `Reassign from Alex to Sarah` | Transfer ownership |
| `Add 3 testing milestones` | Generate new milestones by phase |
| `Delete all blocked milestones` | Bulk remove by status |
| `Set all in progress progress to 50` | Bulk progress update |

### Attaching Documents
Click **📁 Documents** in the sidebar to attach links to:
- Google Docs, Sheets, Slides, Forms
- Figma, Miro, Notion, Confluence
- GitHub repos, Jira tickets, Loom videos
- PDFs or any URL

Documents can be categorized and linked to specific milestones.

## 🏗️ Architecture

This is a **single HTML file** with zero external dependencies (except SheetJS for Excel import). Everything is:
- **Client-side** — no server, no API calls
- **localStorage** — data persists in the browser
- **Shareable via URL** — project data encoded in the URL hash

## 🤝 Contributing

Contributions are welcome! Some ideas:
- [ ] Real-time collaboration via WebSocket/Firebase
- [ ] User authentication
- [ ] Gantt chart drag-to-resize
- [ ] Email notifications
- [ ] Calendar integrations (Google Calendar, Outlook)
- [ ] Export to Google Slides API
- [ ] Dark mode toggle
- [ ] Mobile-optimized layout

## 📄 License

MIT License — use it however you want.

---

Built with ❤️ using [Goose](https://github.com/block/goose) by Block
