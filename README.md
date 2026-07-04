# 🌍 Changes to Adding a Tenant to the CIA Database

> **Last Updated:** July 2026

## 📖 Overview

Two new fields have been added to the OPS JIRA install request:

- 🌍 **YPLM Customer Country**
- 📍 **YPLM Customer Region**

---

## 🖼️ OPS JIRA Request

Replace the placeholder image with your screenshot.

<p align="center">
  <img src="images/jira-fields.png" width="90%">
</p>

---

## 🚀 Option 1 – Manual Jenkins Job

```text
INSTALL - STEP 1 - ADD NEW CUSTOMER INTO CIA DB
```

1. Open the Jenkins job.
2. Enter tenant details.
3. Populate Customer Country and Customer Region.
4. Verify details.
5. Run the job.

<p align="center">
  <img src="images/manual-jenkins-job.png" width="90%">
</p>

---

## ⚡ Option 2 – Jenkins Job (From JIRA)

```text
INSTALL - STEP 1 - ADD NEW CUSTOMER INTO CIA DB - FROM JIRA
```

Provide:
- Base Name
- JIRA Ticket Number

The job automatically retrieves Customer Country and Customer Region.

<p align="center">
  <img src="images/from-jira-job.png" width="90%">
</p>

---

## 🔄 Process Flow

```text
OPS JIRA Request
      │
      ▼
Customer Country & Region
      │
      ▼
Choose Jenkins Job
 ┌──────────────┐
 ▼              ▼
Manual      From JIRA
 │              │
Manual      Auto Fetch
 └─────┬────────┘
       ▼
 CIA Database Updated
```

## 📌 Notes

- Applies to all future customer installations.
- Keep screenshots inside the `images` folder.
