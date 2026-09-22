# 🚨 Resiliai Engage: AI-Powered & Gamified Disaster Response Platform

> **ServiceNow University Hackathon India 2025 Submission**
> **Team:** SixNow Coders — Pragati Engineering College, Surampalem, Andhra Pradesh
> **My Role:** ServiceNow Developer (Back-end)

---

## 📌 Overview

**Resiliai Engage** is an AI-powered and gamified disaster response platform built on **ServiceNow** to improve coordination between authorities, volunteers, and citizens during natural disasters.

During emergencies, fragmented communication and delayed information can lead to inefficient resource allocation and slower response times. Resiliai Engage addresses this problem through a centralized platform that combines:

* 🤖 Generative AI
* ⚡ Automated workflows
* 📱 Citizen and volunteer engagement
* 🏆 Gamification
* 📊 Real-time dashboards
* 🔔 Automated notifications and task assignment

The platform acts as a centralized command system for collecting incident information, generating situational awareness, assigning response tasks, and tracking disaster response activities.

---

## ✨ Key Features

### 🤖 AI-Powered Situational Awareness

Generative AI processes information from citizen reports, alerts, and other data sources to generate concise **Situational Awareness Reports**.

This helps authorities quickly understand:

* Incident type
* Severity
* Location
* Required resources
* Priority of response

---

### ⚙️ Automated Task Orchestration

The platform converts disaster information into actionable response tasks.

Using **Flow Designer**, tasks can be automatically:

* Created
* Prioritized
* Assigned
* Routed to volunteers
* Updated based on task status

---

### 🏆 Gamified Community Engagement

To encourage citizens and volunteers to actively participate during emergencies, the platform includes a gamification system.

Participants can earn:

* ⭐ Points
* 🏅 Badges
* 🏆 Leaderboard rankings

Example badges include:

* **First Responder**
* **Lifesaver**
* **Emergency Reporter**

Points and badges are awarded for activities such as verified incident reporting and successful completion of response tasks.

---

### 📱 Multi-Channel Incident Reporting

Citizens can report incidents through:

* Service Portal
* ServiceNow Mobile App

Reports can include:

* Incident details
* Location
* Photos
* Videos
* Other relevant information

---

### 📊 Centralized Command & Control Dashboard

Authorities can monitor disaster response activities through a centralized dashboard.

The dashboard provides information about:

* 🚨 Active incidents
* 🔥 Incident severity
* 📍 Locations
* 👥 Volunteer availability
* 📦 Resource allocation
* 📈 Response metrics
* 🏆 Gamification leaderboards

---

# 🏗️ Architecture

```text
                 ┌──────────────────────────┐
                 │      Citizen / Volunteer │
                 │        Applications      │
                 └────────────┬─────────────┘
                              │
                              ▼
                 ┌──────────────────────────┐
                 │   Incident Submission    │
                 │ Service Portal / Mobile  │
                 └────────────┬─────────────┘
                              │
                    ┌─────────┴─────────┐
                    ▼                   ▼
          ┌─────────────────┐   ┌─────────────────┐
          │ Gamification    │   │ Incident Data   │
          │ Engine          │   │ & Attachments   │
          └────────┬────────┘   └────────┬────────┘
                   │                     │
                   │                     ▼
                   │          ┌─────────────────────┐
                   │          │ AI Situational      │
                   │          │ Synthesis Engine    │
                   │          └──────────┬──────────┘
                   │                     │
                   │                     ▼
                   │          ┌─────────────────────┐
                   │          │ Generative AI       │
                   │          │ Response Planning   │
                   │          └──────────┬──────────┘
                   │                     │
                   │                     ▼
                   │          ┌─────────────────────┐
                   └─────────►│ Flow Designer       │
                              │ Task Orchestration   │
                              └──────────┬──────────┘
                                         │
                                         ▼
                              ┌─────────────────────┐
                              │ Volunteer Task      │
                              │ Assignment & Alerts │
                              └──────────┬──────────┘
                                         │
                                         ▼
                              ┌─────────────────────┐
                              │ Command & Control   │
                              │ Dashboard           │
                              └─────────────────────┘
```

---

# 🔄 Working Procedure

### 1. 📝 Incident Reporting

Citizens submit disaster-related incidents through the Service Portal or Mobile App.

The report may contain:

* Incident description
* Location
* Severity
* Images
* Videos
* Additional information

The system records the incident in the appropriate ServiceNow table.

---

### 2. 🤖 AI Situational Synthesis

Server-side logic and business rules process incoming incident information.

The Generative AI component can consolidate multiple reports into a **Situational Awareness Report**, helping authorities understand the overall situation.

---

### 3. 🧠 Response Plan Generation

Based on the synthesized information, the AI component generates a proposed response plan.

The plan can identify:

* Required actions
* Priority
* Required resources
* Suitable volunteers
* Response tasks

---

### 4. ⚡ Automated Task Assignment

**Flow Designer** automates the creation and assignment of response tasks.

Tasks can be routed according to factors such as:

* Volunteer skills
* Availability
* Location
* Incident priority

Notifications are sent to relevant volunteers.

---

### 5. 🏅 Gamification

When citizens submit verified reports or volunteers accept and complete tasks, the gamification engine updates their metrics.

Participants can receive:

```text
Points → Badges → Leaderboard Position
```

---

### 6. 📊 Real-Time Monitoring

Authorities can monitor the overall disaster response through centralized dashboards.

Task updates and incident status changes are reflected in the dashboard, providing a consolidated view of ongoing operations.

---

# 🧰 Technology Stack

| Technology / Component   | Usage                                       |
| ------------------------ | ------------------------------------------- |
| **ServiceNow PDI**       | Development environment                     |
| **App Engine Studio**    | Application development                     |
| **Service Portal**       | Citizen-facing interface                    |
| **ServiceNow Mobile**    | Mobile incident and task management         |
| **Flow Designer**        | Workflow automation                         |
| **Business Rules**       | Server-side business logic                  |
| **Notifications**        | Emergency alerts and updates                |
| **Custom Tables**        | Disaster management data model              |
| **Generative AI**        | Situational synthesis and response planning |
| **Dashboards & Reports** | Analytics and monitoring                    |
| **IntegrationHub**       | External data/integration simulation        |

---

# 🗄️ Data Model

The application uses custom ServiceNow tables to manage disaster response information.

### Core Tables

```text
Incidents
    │
    ├── Incident details
    ├── Location
    ├── Severity
    └── Status

Volunteers
    │
    ├── Skills
    ├── Availability
    └── Location

Tasks
    │
    ├── Assigned volunteer
    ├── Priority
    ├── Status
    └── Completion details

Resources
    │
    ├── Resource type
    ├── Availability
    └── Allocation

Gamification Metrics
    │
    ├── Points
    ├── Badges
    └── Leaderboard position
```

---

# 👨‍💻 My Contribution

### **Yarlapati Venkata Naga Durga Varun**

**ServiceNow Developer — Back-end**

My primary responsibilities included:

* Designing and configuring custom ServiceNow tables
* Developing server-side business logic
* Creating and configuring workflows
* Implementing Flow Designer automation
* Developing task assignment logic
* Implementing gamification mechanics
* Configuring points and badge-related functionality
* Supporting incident and volunteer data management
* Integrating different components of the ServiceNow application

---

# 👥 Team

| Team Member                            | Role                             |
| -------------------------------------- | -------------------------------- |
| **Rajeev Boddu**                       | Team Leader & Solution Architect |
| **Yarlapati Venkata Naga Durga Varun** | ServiceNow Developer — Back-end  |
| **Sabbarapu Kumar Ganesh**             | ServiceNow Developer — Front-end |
| **Jenna Meghanadh**                    | AI/NLU Specialist                |
| **Vignesh Mullangi**                   | Data & Reporting Specialist      |
| **Vennapu Lingeswara Rao**             | QA & Documentation               |

---

# 🎯 Project Objectives

Resiliai Engage was designed to:

* Reduce delays in disaster response
* Centralize emergency information
* Improve coordination between stakeholders
* Automate repetitive response workflows
* Improve volunteer utilization
* Encourage citizen participation
* Provide real-time operational visibility
* Support faster and more structured decision-making

---

# 🚀 Future Enhancements

Potential future improvements include:

* 🌐 Integration with live weather APIs
* 📍 Real-time GPS-based volunteer tracking
* 🛰️ Satellite and geospatial disaster data
* 🤖 Advanced AI-based resource optimization
* 📲 Push notifications
* 🗺️ Interactive disaster heat maps
* 🔗 Integration with government emergency systems
* 📊 Predictive disaster analytics
* 🧠 AI-powered incident severity classification

---

# 🏆 Hackathon

**ServiceNow University Hackathon India 2025**

**Project:** Resiliai Engage
**Team:** SixNow Coders
**Institution:** Pragati Engineering College, Surampalem, Andhra Pradesh

The project demonstrates how **ServiceNow, Generative AI, workflow automation, and gamification** can be combined to build a centralized platform for disaster response and community engagement.

---

## 📄 Documentation

The project documentation covers:

* Problem statement
* Proposed solution
* System architecture
* ServiceNow implementation
* Data model
* Workflow design
* AI integration concept
* Gamification mechanism
* Testing and demonstration workflow

---

## ⭐ Keywords

`ServiceNow` `Generative AI` `Disaster Management` `Flow Designer` `Business Rules` `Service Portal` `ServiceNow Mobile` `App Engine Studio` `IntegrationHub` `Workflow Automation` `Gamification` `Incident Management` `Emergency Response`
