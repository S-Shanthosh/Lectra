# 🛡️ WAF Automation — Quick Run Guide

> **Fast setup → Activate → Run → Check Excel** 🚀

---

## 📁 Folder Structure

```text
Automation Scripts\
│
├── waf_report.py          ← 🐍 Python automation script
├── waf-report.xlsx        ← 📊 Main Excel file
├── venv\                  ← 🐍 Python virtual environment
└── Testing\              ← 🧪 Test/sample files
```

### ⚠️ Important

- Keep **`waf-report.xlsx` OUTSIDE `venv`**
- Keep the Excel file in the **same folder as the Python script**
- The Excel workbook must contain a sheet named **`raw_report`**
- Do not rename or move `venv` unless you also update the activation command

---

## 📍 Working Path

```text
H:\My Drive\Lectra KT and Docs\Automation Scripts
```

Go there:

```cmd
cd /d "H:\My Drive\Lectra KT and Docs\Automation Scripts"
```

---

## 🐍 Activate Virtual Environment

```cmd
venv\Scripts\activate
```

You should see:

```text
(venv) H:\My Drive\Lectra KT and Docs\Automation Scripts>
```

✅ **`(venv)` = Virtual environment is active**

---

## ▶️ Run WAF Python Script

With `(venv)` active:

```cmd
python waf_report.py
```

---

## 📊 Excel Requirement

The workbook must be:

```text
waf-report.xlsx
```

and located here:

```text
H:\My Drive\Lectra KT and Docs\Automation Scripts\waf-report.xlsx
```

Required input sheet:

```text
raw_report
```

### 🔄 Basic Flow

```text
raw_report
     ↓
🐍 waf_report.py
     ↓
📊 Process WAF data
     ↓
📈 Update waf-report.xlsx
```

---

## ⚡ One-Shot Startup

From any normal CMD:

```cmd
cd /d "H:\My Drive\Lectra KT and Docs\Automation Scripts"
venv\Scripts\activate
python waf_report.py
```

---

## 🔎 Quick Checks

### Check files

```cmd
dir
```

### Check Python

```cmd
python --version
```

### Check which Python is active

```cmd
where python
```

It should point inside:

```text
...\Automation Scripts\venv\Scripts\python.exe
```

---

## 🚨 Common Mistakes

| ❌ Don't | ✅ Do |
|---|---|
| Put Excel inside `venv` | Keep Excel beside the `.py` file |
| Run without activating `venv` | Activate `venv` first |
| Rename `raw_report` sheet | Keep it exactly `raw_report` |
| Run from another folder | `cd` to Automation Scripts first |
| Rename the workbook incorrectly | Use `waf-report.xlsx` |

---

## 🏁 Remember

**📍 PATH → 🐍 ACTIVATE → 📊 CHECK EXCEL → ▶️ RUN**

```cmd
cd /d "H:\My Drive\Lectra KT and Docs\Automation Scripts"
venv\Scripts\activate
python waf_report.py
```

> 💡 **Keep the setup simple: script + Excel together, virtual environment separate.**
