# Resiliai Engage: AI-Powered & Gamified Disaster Response Platform

> **ServiceNow University Hackathon India 2025 Submission**  
> **Team:** SixNow Coders (Pragati Engineering College, Surampalem, AP)[cite: 1]  
> **Role (Yarlapati Venkata Naga Durga Varun):** ServiceNow Developer (Back-end)[cite: 1]

---

## 📌 Executive Summary

During natural disasters, coordination among authorities, volunteers, and citizens is often fragmented, causing critical delays and inefficient resource allocation[cite: 1]. **Resiliai Engage** addresses this challenge by providing a centralized, automated ServiceNow platform[cite: 1]. 

The platform acts as a central nervous system for disaster management, leveraging **Generative AI** as a cognitive assistant to aggregate incident reports, synthesize real-time situational awareness, and dynamically orchestrate response workflows[cite: 1]. To maintain continuous engagement during crises, the platform integrates a dynamic **gamification engine** that rewards citizens and volunteers with points, badges, and leaderboard rankings for active participation[cite: 1].

---

## ✨ Key Features & Innovations

* **AI-Powered Situational Synthesis:** A Generative AI engine processes unstructured data from citizen forms, social feeds, and alerts to generate concise, actionable "Situational Awareness Reports" in real time, eliminating information overload[cite: 1].
* **Automated Task Orchestration:** Converts synthesized situational reports into optimal response plans, dynamically generating and routing actionable tasks via Flow Designer[cite: 1].
* **Gamified Community Engagement:** Built-in rewards system awarding points, badges (e.g., *"First Responder"*, *"Lifesaver"*), and leaderboard placements to citizens for verified reporting and volunteers for completing high-priority tasks[cite: 1].
* **Multi-Channel Input:** Accessible via a custom Service Portal and Mobile App for on-the-go incident submission with photo/video attachments[cite: 1].
* **Centralized Command & Control Dashboard:** Single-pane-of-glass monitoring interface for authorities showing incident severity maps, resource allocation, volunteer engagement, and live leaderboards[cite: 1].

---

## 🛠️ Architecture & Working Procedure

[Citizen Incident Submission] ──► [Gamification Points Awarded]
│
▼
[AI Situational Synthesis Engine] ──► [Generative AI Response Plan]
│
▼
[Central Dashboard Analytics] ◄── [Automated Task Routing & Dispatch]


1. **Reporting:** Citizens submit structured reports via the Service Portal/Mobile App and instantly receive points[cite: 1].
2. **AI Synthesis:** Server-side scripts/Business Rules aggregate report details into a consolidated Situational Awareness Report[cite: 1].
3. **Plan Generation & Tasking:** Generative AI creates an optimal response plan, automatically translating it into tasks[cite: 1].
4. **Intelligent Dispatch:** Flow Designer assigns tasks to volunteers based on location and skills, issuing notification alerts and "First Responder" badges upon task acceptance[cite: 1].
5. **Real-time Updates & Completion:** Volunteers update task statuses via mobile interface; task completion updates central dashboards and awards completion badges[cite: 1].

---

## 🧰 Tech Stack & ServiceNow Components

* **Platform Environment:** ServiceNow Personal Developer Instance (PDI)[cite: 1]
* **Development & UI:** App Engine Studio, Service Portal, ServiceNow Mobile App[cite: 1]
* **Workflow & Automation:** Flow Designer, Server-side Business Rules, Notifications[cite: 1]
* **Data Model:** Custom Tables (`Incidents`, `Volunteers`, `Tasks`, `Resources`, `Gamification_Metrics`)[cite: 1]
* **Reporting & Integrations:** Dashboards & Reports, IntegrationHub (simulated social feeds/weather API)[cite: 1]

---

## 👥 Team Structure & Roles

| Team Member | Role & Responsibilities |
| :--- | :--- |
| **Rajeev Boddu** | Team Leader & Solution Architect[cite: 1] |
| **Yarlapati Venkata Naga Durga Varun** | **ServiceNow Developer (Back-end):** Core workflows, Custom Tables, server-side business logic, Flow Designer, and gamification mechanics[cite: 1]. |
| **Sabbarapu Kumar Ganesh** | **ServiceNow Developer (Front-end):** Service Portal, Mobile UI/UX, and gamification visual interfaces[cite: 1]. |
| **Jenna Meghanadh** | **AI/NLU Specialist:** AI logic design, NLU configuration, and Generative AI mock-ups[cite: 1]. |
| **Vignesh Mullangi** | **Data & Reporting Specialist:** Dynamic Command & Control dashboards, analytics, and metric structures[cite: 1]. |
| **Vennapu Lingeswara rao** | **QA & Documentation:** Solution testing, documentation compile, and demo workflow preparation[cite: 1]. |

---

## 📄 References & Documentation

* Project proposal and architecture submitted for **ServiceNow University Hackathon India 2025**[cite: 1].
* Included project documentation outlines implementation phases, data model design, and step-by-step working procedure[cite: 1].
