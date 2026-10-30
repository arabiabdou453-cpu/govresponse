# GovResponse — Real-Time Emergency Operations Center (EOC) Platform

[![GitHub Pages](https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-brightgreen?style=for-the-badge&logo=github)](https://arabiabdou453-cpu.github.io/govresponse/)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)](LICENSE)
[![Standards: NIMS & ICS](https://img.shields.io/badge/Standards-NIMS%20%7C%20ICS%20%7C%20SEMS-orange?style=for-the-badge)](https://www.fema.gov/emergency-managers/nims)
[![Compliance: FEMA & Cal OES](https://img.shields.io/badge/Compliance-FEMA%20PA%20%7C%20Cal%20OES-red?style=for-the-badge)](https://www.caloes.ca.gov/)

A mission-critical, browser-based Emergency Operations Center (EOC) software platform designed for emergency managers, county OES teams, municipalities, and disaster response organizations to manage incidents end-to-end — from tactical mapping and resource requests to automated FEMA Public Assistance cost recovery.

---

## 🌟 Live Demo

- **Public Live Application:** [https://arabiabdou453-cpu.github.io/govresponse/](https://arabiabdou453-cpu.github.io/govresponse/)
- **Source Repository:** [https://github.com/arabiabdou453-cpu/govresponse](https://github.com/arabiabdou453-cpu/govresponse)

---

## 🏛️ Platform Architecture & Overview

GovResponse replaces fragmented spreadsheets, paper ICS forms, and disparate radio logs with a unified, real-time command canvas accessible on any device — whether in the primary EOC, an alternate facility, or field incident command posts.

```
+---------------------------------------------------------------------------------------+
|                         GovResponse Unified Incident Ecosystem                        |
+---------------------------------------------------------------------------------------+
         │                                   │                               │
         ▼                                   ▼                               ▼
+───────────────────────────+   +───────────────────────────+   +───────────────────────────+
|     Tactical Operations   |   |     ICS & SEMS Command    |   |     Disaster Finance      |
| • Geospatial Incident Map |   | • Automated ICS 201-214   |   | • FEMA Cost Recovery      |
| • Evacuation Perimeters   |   | • NIMS Incident Org Chart |   | • Force Account Labor     |
| • Shelter Capacity Matrix |   | • Cal OES After-Action    |   | • Equipment Rate Tables   |
| • Needs & Resource Triage |   | • Operational Period IAP  |   | • Audit-Ready Dossiers    |
+───────────────────────────+   +───────────────────────────+   +───────────────────────────+
         │                                   │                               │
         └───────────────────────────────────┼───────────────────────────────┘
                                             ▼
+---------------------------------------------------------------------------------------+
|                     Multi-Agency Interoperability & Field Synchronization            |
|       • FirstNet / Cellular Resilient  • Offline PWA Cache  • Role-Based Access       |
+---------------------------------------------------------------------------------------+
```

---

## 🚀 Key Modules & Functional Capabilities

### 1. Unified Tactical Map & Spatial Situational Awareness
- **Dynamic Incident Boundaries:** Real-time perimeter mapping for wildfires, floods, HazMat plumes, and severe weather tracks.
- **Evacuation Zone Management:** Triage Order, Warning, and Shelter-in-Place zones with population impact estimates and real-time shelter capacity gauges.
- **Resource Placement:** Real-time visual tracking of deployed heavy equipment, strike teams, mutual aid assets, and staging areas.

### 2. Standardized ICS & SEMS Workflow Automation
- **Incident Command System (ICS) Standard Forms:** Native generation of core incident documents including:
  - **ICS 201:** Incident Briefing
  - **ICS 202:** Incident Objectives
  - **ICS 203:** Organization Assignment List
  - **ICS 204:** Assignment List
  - **ICS 205:** Incident Radio Communications Plan
  - **ICS 206:** Medical Plan
  - **ICS 214:** Unit Activity Log
- **Incident Action Plan (IAP) Builder:** One-click compilation of operational period IAP packets for briefings and state agency submission.
- **California SEMS Alignment:** Structured for Field, Local Government, Operational Area, Regional, and State levels.

### 3. Resource Requests & Unmet Needs Triage
- **Logistics Fulfillment Pipeline:** Track resource lifecycles from initial Request → Sourcing → Mobilization → Staging → Demobilization.
- **Inter-Agency Mutual Aid:** Clear routing for mutual aid requests across adjoining cities, counties, and Cal OES regions.

### 4. FEMA Cost Recovery & Cal OES After-Action Reporting
- **FEMA Public Assistance (PA) Compliance:** Capture audit-ready expenditure records categorized by FEMA work types (Category A Debris Removal, Category B Emergency Protective Measures, etc.).
- **Labor & Equipment Tracking:** Automatically calculate costs using FEMA Schedule of Equipment Rates and standard Force Account labor formulas.
- **Automated After-Action Reports (AAR):** Auto-generate chronological event logs and lessons-learned matrices required for state and federal reimbursement.

---

## 💻 Tech Stack & Deployment Options

- **Frontend:** Next.js (App Router), Tailwind CSS design system, dark-mode first command center palette, responsive grid/flex architecture.
- **Server:** Zero-dependency Node.js HTTP server (`server.js`) with automatic static routing and SPA client-side fallback.
- **Typography & Assets:** Offline-ready DM Mono, Syne, and DM Sans web fonts with SVG tactical iconography.

---

## 🛠️ Quick Start Guide

### Prerequisites
- Node.js (v18.0 or higher recommended)
- Git

### Installation & Local Run

1. **Clone the repository:**
   ```bash
   git clone https://github.com/arabiabdou453-cpu/govresponse.git
   cd govresponse
   ```

2. **Start the local server:**
   ```bash
   npm start
   ```

3. **Open the browser:**
   ```
   http://localhost:3000
   ```

*(Alternatively, run with any standard static server such as `npx serve .` or Python `python -m http.server 3000`.)*

---

## 📁 Repository Structure

```
govresponse/
├── _next/                         # Compiled Next.js production chunks & static assets
│   └── static/
│       ├── chunks/                # Optimized modular JS bundles
│       ├── css/                   # Tailored command center stylesheets
│       └── media/                 # Offline-cached high-legibility web fonts
├── 404.html                       # Fallback error and deep-link handler
├── icon.svg                       # Tactical platform vector icon
├── index.html                     # Pre-rendered incident management application
├── logo.png                       # Official GovResponse brand mark
├── package.json                   # Project metadata and zero-dependency scripts
├── server.js                      # High-efficiency static HTTP server
├── LICENSE                        # MIT License
└── README.md                      # Comprehensive platform documentation
```

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).
