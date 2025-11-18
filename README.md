# PlanApproval Messenger

A modern, three-pane messenger UI prototype designed for the **Plan Approval** and **Technical Teams** at Asia Classification Society.  
This project focuses on a clean, production-ready front-end that can later be wired to a real-time backend (WebSockets / REST).

> Built with React, TypeScript, Vite, and Tailwind CSS. The initial layout was generated from a Magic Patterns Vite template and then customized for the PlanApproval use case. :contentReference[oaicite:0]{index=0}

---

## ✨ Features

- **Three-pane messenger layout**
  - Left: conversation list (teams, direct messages, unread badges)
  - Center: active chat, message bubbles, timestamps, attachments
  - Right: information panel for pinned media, files, and manager notes

- **Conversation list**
  - Support for *Direct* vs *Team* threads
  - Role labels (e.g. Executive / Technician)
  - Online / away presence indicators
  - Unread counters and last-message preview

- **Chat view**
  - Distinct styling for executive vs technician messages
  - Message timestamps and compact layout for long threads
  - Support for message attachments (images / files) with metadata

- **Pinned resources panel**
  - Sections for:
    - Pinned media (screenshots, diagrams, etc.)
    - Files (documents, PDFs, drawings)
    - Management notes / instructions
  - Designed to help engineers keep context while chatting

- **Developer-friendly front-end**
  - Pure front-end, no backend vendor lock-in
  - Easy to connect to REST / WebSocket APIs
  - Tailwind utility classes for fast customization

---

## 🧱 Tech Stack

- **Framework:** React + TypeScript
- **Bundler / Dev Server:** Vite :contentReference[oaicite:1]{index=1}  
- **Styling:** Tailwind CSS + utility-first design
- **Tooling:**
  - ESLint / TypeScript configuration via Vite template
  - PostCSS + Tailwind pipeline

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/alirazi1992/PlanApproval_-Messenger-.git
cd PlanApproval_-Messenger-

```

## Project Structer (high- level) 

PlanApproval_-Messenger-/

├─ src/

│  ├─ App.tsx          # Main messenger layout

│  ├─ main.tsx        # React entry point

│  ├─ components/     # Reusable UI components (layout, buttons, icons, etc.)

│  └─ ...             # Styles, hooks, helpers

├─ index.html

├─ package.json

├─ tailwind.config.js

├─ postcss.config.js

└─ vite.config.ts

----

## 🧩 How to Integrate with a Backend (Ideas)

This repository currently focuses on UI. To connect it to a real system, you can:

Add API calls (REST) to load:

Conversation list

Message history

Pinned media/files

Use WebSockets (or Socket.IO, SignalR, etc.) for:

Real-time messaging

Typing indicators

Presence updates

Plug in your own:

Authentication (JWT / session)

Authorization (roles: admin, executive, technician)


## 🛠 Scripts

Common npm scripts (see package.json):

- `npm run dev` – Start development server

- `npm run build` – Create production build

- `npm run preview` – Preview the production build locally

  ---

## 🗺 Roadmap / Next Steps

- Connect to real PlanApproval API for:

     - Tickets / cases <> chat linkage

     - Plan document references in threads

- Add message search & filters

- Add dark theme and user preferences

- Add per-thread pinned notes & media management
