# 🌍 Changes to Adding a Tenant to the CIA Database

> **Last Updated:** July 2026

---

# 📖 Overview

To better identify customer locations, two new fields have been added to the **YPLM New Cloud Customer Install Request** in the OPS JIRA Portal.

The new fields are:

- 🌍 **YPLM Customer Country**
- 📍 **YPLM Customer Region**

These values must now be populated in the CIA database whenever a new tenant is created.

---

# 🖼️ OPS JIRA Request

> 📷 **Snapshot 1**
>
> *(Insert screenshot of the OPS JIRA request highlighting the Customer Country and Customer Region fields.)*

---

# 🚀 Option 1 – Manual Jenkins Job

```text
INSTALL - STEP 1 - ADD NEW CUSTOMER INTO CIA DB
```

## Steps

1. Open the Jenkins job.
2. Enter the required tenant details.
3. Populate:
   - 🌍 Customer Country
   - 📍 Customer Region
4. Verify all information.
5. Execute the job.

---

## 🖼️ Manual Jenkins Job

> 📷 **Snapshot 2**
>
> *(Insert screenshot here.)*

---

# ⚡ Option 2 – Jenkins Job (From JIRA)

```text
INSTALL - STEP 1 - ADD NEW CUSTOMER INTO CIA DB - FROM JIRA
```

## Required Inputs

- Base Name
- JIRA Ticket Number

Automatically retrieves:

- ✅ Customer Country
- ✅ Customer Region
- ✅ Remaining customer information

---

## 🖼️ From JIRA Jenkins Job

> 📷 **Snapshot 3**
>
> *(Insert screenshot here.)*

---

# 🔄 Process Flow

```text
OPS JIRA Install Request
        │
        ▼
Customer Country & Customer Region
        │
        ▼
Choose Jenkins Job
 ┌───────────────┐
 ▼               ▼
Manual       From JIRA
 │               │
Manual Entry  Auto Fetch
 └───────┬───────┘
         ▼
 CIA Database Updated
```

---

# ✅ Best Practices

- Verify Customer Country and Customer Region.
- Enter them manually when using the manual Jenkins job.
- Use the FROM JIRA job whenever possible.
- Verify the job completes successfully.

---

# 📌 Notes

- Applies to all future customer installations.
- Improves customer location tracking.
- Ensures consistent CIA database records.
