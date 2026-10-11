<div align="center">

# ⚙️ Automation & Data Intelligence
### **Enterprise Workflow Orchestration, Scraping & Google Sheet Enrichment**

[![Platform](https://img.shields.io/badge/Platform-n8n-FF6D5A?style=for-the-badge&logo=n8n&logoColor=white)](https://n8n.io/)
[![Language](https://img.shields.io/badge/Language-JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Integrations](https://img.shields.io/badge/Integrations-Google_Sheets-34A853?style=for-the-badge&logo=googlesheets&logoColor=white)](https://developers.google.com/sheets/api)
[![Workflows](https://img.shields.io/badge/Workflows-6_Pipelines-blue?style=for-the-badge)](Project/)
[![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)](LICENSE)

**End-to-end automated pipelines for B2B prospecting, domain intelligence, company metadata enrichment, and real-time spreadsheet synchronization.**

---

[Explore Pipelines](#-core-automation-pipelines) • [7-Day Engineering Sprint](#-7-day-engineering-sprint) • [Project Structure](#-project-structure) • [Tech Stack](#-tech-stack)

</div>

---

## 📖 Overview
**Automation & Data Intelligence** is an end-to-end automation suite engineered with **n8n**. Designed to transform raw domain links and unstructured lead lists into verified, actionable databases, it orchestrates continuous crawling, intelligent regex pattern matching, email MX validation, and asynchronous Google Sheets updates without manual intervention.

---

## 🚀 Core Automation Pipelines

### 1. 🎯 Lead Generation Pipeline
- **Form-Triggered Onboarding:** Accepts user spreadsheet links via a self-hosted web form.
- **Automated Domain Crawling:** Scrapes executive contact points, company summaries, and social media handles.
- **Google Sheet Sync:** Automatically writes verified email addresses and company metrics back to target rows.

### 2. 🏢 Company Enrichment from Google Sheet
- **Deep Domain Reconnaissance:** Fetches WHOIS data, industry sector, headquarters, employee headcounts, and tech stacks.
- **Anti-Duplication Guard:** Validates existing rows to ensure zero redundant API queries.

### 3. ✅ Sheet Row Verify & Auto-Update
- **Live Row Watcher:** Polls or triggers upon row additions to sanitize phone numbers, format URL schemas, and normalize names.
- **Real-Time Data Hygiene:** Auto-updates rows with standardized formats and timestamped audit flags.

### 4. 🕸️ Website Data Miner (Final)
- **Deep Page Traversal:** Crawls multi-tier internal routes (`/contact`, `/about`, `/team`) to discover buried contact coordinates.
- **Pattern Matching Engine:** Discovers obfuscated mailto links and corporate telephone lines.

---

## 📅 7-Day Engineering Sprint

| Day | Milestone Focus | Deliverable |
| :---: | :--- | :--- |
| **Day 1** | Foundation & Environment Setup | Environment orchestration & architecture design log |
| **Day 2** | Company Enrichment & Email Parsing | `Company Enrichment from Google Sheet.json`, `sheet-_ Mail -_ Update.json` |
| **Day 3** | Resilient Webhook Handlers | Rate limiting, error trapping & retry protocols |
| **Day 4** | Real-Time Sheet Row Verification | `Sheet Row Verify & Auto-Update.json` |
| **Day 5** | End-to-End Lead Generation Engine | `Lead Generation.json` |
| **Day 6** | Deep Website Crawler Architecture | `Website Data Miner.json` |
| **Day 7** | Multi-Tier Crawler Finalization | `Website Data Miner (Final).json` |

---

## 📁 Project Structure

```text
Automation/
├── Project/                    # Production-ready n8n workflow definitions
│   ├── Company Enrichment from Google Sheet.json
│   ├── Lead Generation.json
│   ├── Sheet Row Verify & Auto-Update.json
│   ├── sheet-_ Mail -_ Update.json
│   ├── Website Data Miner.json
│   └── Website Data Miner (Final).json
├── Log/                        # Detailed daily engineering logs & PDF reports
│   ├── Day 1/
│   ├── Day 2/
│   ├── Day 3/
│   ├── Day 4/
│   ├── Day 5/
│   ├── Day 6/
│   └── Day 7/
└── README.md
```

---

## 🛠️ Tech Stack

| Layer | Technology | Purpose |
| :--- | :--- | :--- |
| **Automation Engine** | [n8n](https://n8n.io) | Low-code workflow and node orchestration |
| **Data Synchronization**| Google Sheets API v4 | Bi-directional spreadsheet reading & batch cell writing |
| **Web Crawling** | Cheerio / Headless HTTP Nodes | Fast HTML parsing, meta-tag & link extraction |
| **Scripting & Parsing**| JavaScript (Node.js) | Complex JSON transformation & regex matching |
| **Reporting** | PDF Documentation & Audit Logs | Daily telemetry, process charts & progress logs |

---

## 📄 License
Distributed under the MIT License. See `LICENSE` for more information.

<div align="center">

**Developed with ❤️ by Fuad**  
*Developed by Softece*  
*Automation Ecosystem*

</div>
