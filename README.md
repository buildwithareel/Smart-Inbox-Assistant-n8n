# 📧 Smart Inbox Assistant – AI Email Automation with n8n

![n8n](https://img.shields.io/badge/n8n-Workflow%20Automation-EA4B71?logo=n8n&logoColor=white)

![AI Agent](https://img.shields.io/badge/AI-Agent-blueviolet)

![Google Gmail](https://img.shields.io/badge/Gmail-Integrated-EA4335?logo=gmail&logoColor=white)

![Google Sheets](https://img.shields.io/badge/Google%20Sheets-Integrated-34A853?logo=googlesheets&logoColor=white)

![Level](https://img.shields.io/badge/Level-Intermediate-blue)

![License](https://img.shields.io/badge/License-MIT-green)

# Description 
An AI-powered email automation workflow built with **n8n** that automatically analyzes incoming Gmail messages, classifies emails by category and priority, generates professional draft replies using an AI Agent, routes urgent emails for immediate action, and logs all processed emails into Google Sheets.

## 📑 Table of Contents

- [📌 Project Information](#-project-information)
- [🎯 Project Overview](#-project-overview)
- [❗ Problem Statement](#-problem-statement)
- [💡 Solution](#-solution)
- [🏗️ Workflow Architecture](#️-workflow-architecture)
- [✨ Features](#-features)
- [🤖 AI Agent Prompt](#-ai-agent-prompt)
- [⚙️ Workflow Explanation](#️-workflow-explanation)
- [📸 Screenshots](#-screenshots)
- [🎥 Demo](#-demo)
- [🛠️ Tech Stack](#️-tech-stack)
- [📂 Folder Structure](#-folder-structure)
- [🚀 Installation](#-installation)
- [⚙️ Configuration](#️-configuration)
- [▶️ Usage](#️-usage)
- [📊 Google Sheet Structure](#-google-sheet-structure)
- [🔮 Future Improvements](#-future-improvements)
- [👨‍💻 Author](#-author)
- [📄 License](#-license)

## 📌 Project Information

| Project | Details |
|----------|---------|
| Project Name | Smart Inbox Assistant |
| Platform | n8n |
| Category | AI Email Automation |
| Difficulty | Intermediate |
| AI Model | Google Gemini |
| Trigger | Gmail Trigger |
| Integrations | Gmail, Google Sheets |
| Status | Completed |

## 🎯 Project Overview

Managing emails manually can be time-consuming, especially when important messages need immediate attention while less urgent emails can wait. Businesses and professionals often spend valuable time reading, categorizing, prioritizing, and replying to emails.

The **Smart Inbox Assistant** is an AI-powered automation workflow built with **n8n** that intelligently processes incoming Gmail messages. Using an AI Agent, it automatically classifies each email, assigns a priority level, generates a professional draft reply, routes urgent emails for immediate action, and logs all processed emails into Google Sheets.

This workflow demonstrates how AI and workflow automation can work together to reduce repetitive tasks, improve response times, and streamline email management.

## ❗ Problem Statement

Managing emails manually can quickly become overwhelming, especially when inboxes receive a high volume of messages every day. Users must spend time opening each email, understanding its purpose, determining its urgency, drafting replies, and organizing important conversations.

This repetitive process increases response time, reduces productivity, and increases the risk of overlooking high-priority emails. Businesses and professionals need an efficient solution that can intelligently process emails while reducing manual effort.

## 💡 Solution

The Smart Inbox Assistant automates the complete email processing workflow using AI and n8n.
Whenever a new email arrives in Gmail, the workflow automatically:

- Detects the incoming email.
- Extracts the required email information.
- Uses an AI Agent to analyze the email content.
- Classifies the email into an appropriate category.
- Assigns a priority level (High,Medium, or Low).
- Generates a professional draft reply.
- Sends urgent emails for immediate attention or saves non-urgent replies as drafts.
- Logs every processed email into Google Sheets for tracking and record keeping.

This automation reduces manual effort, improves response consistency, and ensures that important emails receive immediate attention.

## 🏗️ Workflow Architecture

The Smart Inbox Assistant follows a structured automation pipeline that combines Gmail, AI, conditional logic, and Google Sheets to process incoming emails efficiently.

The workflow receives every new Gmail message, extracts the required information, uses an AI Agent to analyze the content, determines the email category and priority, generates a professional draft reply, routes the email based on its priority, and finally records the processed email information in Google Sheets.

## 📊 Workflow Flow

```text
New Email (Gmail)
        │
        ▼
 Gmail Trigger
        │
        ▼
  Edit Fields
        │
        ▼
    AI Agent
(Classify & Prioritize)
        │
        ▼
   Code Node
(Parse AI JSON)
        │
        ▼
     IF Node
     │      │
     │      │
 High   Medium / Low
     │          │
     ▼          ▼
Send Email   Create Draft
     │          │
     └────┬─────┘
          ▼
 Google Sheets
```

## ⚙️ Workflow Explanation

| Step | Node | Purpose |
|------|------|---------|
| 1 | Gmail Trigger | Detects every new incoming Gmail message. |
| 2 | Edit Fields | Extracts and formats the required email information. |
| 3 | AI Agent | Analyzes the email, assigns a category and priority, generates a summary, and creates a professional draft reply. |
| 4 | Code | Parses and validates the AI-generated JSON output. |
| 5 | IF | Routes emails according to their priority level. |
| 6 | Gmail | Sends urgent emails immediately or creates draft replies for medium and low priority emails. |
| 7 | Google Sheets | Stores processed email details for tracking and reporting. |

## 📸 Workflow Architecture

![Workflow](screenshorts/workflow.png)
