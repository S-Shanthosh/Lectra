# 🛡️ WAF Report Generator

Tools available for generating **WAF reports**.

## 🌐 1. HTML + Python — Recommended

**Primary option for report generation.**

👉 [waf_Py_app.html](https://github.com/S-Shanthosh/Lectra/blob/main/WAF/HTML/waf_Py_app.html)

- Browser-based and easy to use.
- ⚠️ Minor **bleeding issues** may occur in a few sheets.
- Easily corrected with a **manual touch-up**.

## 🐍 2. Python — Offline

**Use when offline report generation is required.**

- Runs locally/offline.
- Generates the report reliably.
- ⚠️ Same minor bleeding issues may occur.
- Easily fixed manually.

## 🟨 3. JavaScript — Backup

**Use only when the above two options are unavailable.**

- Intended for urgent situations.
- May struggle with **large datasets (2,000+ lines)**.
- If it fails, delete the sheets containing the **largest datasets** and run again.

> 💡 **Priority:** 🌐 HTML + Python → 🐍 Python → 🟨 JavaScript