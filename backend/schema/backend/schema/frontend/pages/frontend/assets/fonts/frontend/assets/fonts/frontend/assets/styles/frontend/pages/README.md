# 📊 Report Page: Audit-Friendly Documentation

## 🔍 Purpose
This page summarizes system activity (login, updates, password resets) in a clear tabular format, using Lean filters for date range and action type. It supports audit review, traceability, and external export without requiring backend access.

---

## 🎨 UI Standards

- **Font:** `Kanit` — consistent with system-wide branding
- **Color Palette:**
  - Background: `#F5F5DC` (Beige)
  - Buttons: `#3D4C5A` (Blue-gray)
  - Text: `#333333` (Dark gray)

All styles comply with Ebed's locked design palette and minimal audit-focused layout.

---

## 🧱 Layout & Structure

- **Filter Section:**
  - `startDate`, `endDate`: HTML date input for range filtering
  - `actionType`: dropdown with options for login, update, reset
  - `primary-btn`: triggers filtered display

- **Table:**
  - Columns: Time, User, Action, Details
  - Responsive, collapsible, border-visible for readability
  - `<tbody>` is dynamically populated via JS (audit visible)

---

## ⚙️ Functionality Logic

- JS filters mock data based on:
  - Date range comparison via string slice (`YYYY-MM-DD`)
  - Action type match (empty = show all)
- `report.js` does not require backend → audit-safe by default
- Clears old data before render → prevents stale/inconsistent logs

---

## 🛡️ Audit Rationale

| Element        | Rationale                                  |
|----------------|--------------------------------------------|
| No plugin used | Full transparency; avoids hidden logic     |
| Mock data      | Reviewer can verify frontend before backend |
| Portable HTML  | Can export or preview without build tools  |
| Locked style   | Prevents drift from approved UI baseline   |

---

## 📦 Ready for External Review

This page is complete and stable for review by auditors, stakeholders, or external system architects.  
No dependencies, no dynamic backend — safe for staging, demo, or export.

