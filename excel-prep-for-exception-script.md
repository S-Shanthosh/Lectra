# 📊 Excel Prep Workflow — Pre-Script Checklist

> 🎯 **Goal:** Get your Athena CSV export fully cleaned, formatted, and table-free so it's 100% ready for the exception-handling script.

---

## 🟢 Step 1 — Import via Power Query
> 📂 `Data` → `Get Data` → `From File` → `From Text/CSV`

- Select your **Athena CSV** file
- ⚠️ In the preview dialog, click **`Transform Data`** — ❌ **NOT** `Load`!

---

## 🔵 Step 2 — Fix the `referenceno` Column Type
> 🛠️ In the Power Query Editor:

- Click the **`123`** icon on the **`referenceno`** column header
- Select **`Text`**
- Choose **`Replace current`** ✅

💡 *This prevents Excel from messing up long reference numbers (no more scientific notation or dropped leading zeros!)*

---

## 🟣 Step 3 — Load & Convert Table to Range
> 🏠 Back in Excel:

- Click anywhere inside the green/white table
- Go to **`Table Design`** tab (far right of ribbon)
- Click **`Convert to Range`**
- Confirm with **`Yes`** ✅

🎉 Your data is now a normal range — no more table formatting quirks!

---

## 🟡 Step 4 — Format Painter for ALL Columns *(except cdate & timestamp)*

- 🖌️ **Double-click** Format Painter to "lock" it on
- Pick **any white/blank-formatted column** as your source
- Click across **all columns EXCEPT** `cdate` and `timestamp`
- Press `Esc` when done

---

## 🟠 Step 5 — Format Painter for `cdate` & `timestamp` Columns

- 🖌️ Use Format Painter again
- This time, apply the **date/timestamp-specific formatting** to just these two columns

---

## 🔴 Step 6 — Final Cleanup

- ✅ Select **all cells** (`Ctrl + A`)
- ✅ Confirm **"No table"** is applied (no banded rows, no table styling)

---

## ✅ Step 7 — Ready for Scripting! 🚀

> 🎊 Your Excel sheet is now **clean, formatted, and script-ready**.
> Run your **exception-handling script** with confidence! 💪

---

### 📝 Quick Reference Card

| Step | Action | Shortcut/Path |
|------|--------|---------------|
| 1️⃣ | Import CSV | `Data → Get Data → From File → From Text/CSV` |
| 2️⃣ | Fix referenceno type | `123 icon → Text → Replace current` |
| 3️⃣ | Convert to Range | `Table Design → Convert to Range → Yes` |
| 4️⃣ | Format Painter (all cols) | Double-click 🖌️, skip `cdate`/`timestamp` |
| 5️⃣ | Format Painter (date cols) | Apply to `cdate` & `timestamp` only |
| 6️⃣ | Final check | `Ctrl+A` → confirm no table styling |
| 7️⃣ | Done! | Run exception script ⚡ |

---

📌 *Save this file in your repo for quick reference before every script run!*
