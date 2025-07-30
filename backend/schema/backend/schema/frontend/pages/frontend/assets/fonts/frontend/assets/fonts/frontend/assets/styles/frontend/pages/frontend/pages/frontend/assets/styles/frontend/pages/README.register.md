# Ebed Register Page Overview

## 🧱 Structure
- `register.html` — Registration page with essential fields
- `../assets/fonts/kanit.css` — Locked Kanit font from Google Fonts
- `../assets/fonts/logo-font.css` — Style for system name “Ebed”
- `../assets/styles/register.css` — UI styling: beige background, dark gray text, blue-gray button

## 📋 Field Justification
- **Username** — Required for login ID; links with audit trail
- **Password** — Essential for authentication; handled securely in backend
- **Full name** — Non-redundant metadata; used for profile and reviewer traceability

No role, ID, or status fields here — those are handled in controlled admin schema

## 🎨 Design Tokens
- **Background**: `#F5F5DC` (Beige)
- **Text**: `#333333` (Dark gray)
- **Primary Button**: `#3D4C5A` (Blue-gray)
- **Font**: Kanit (locked)

## ✅ Audit Notes
- Style separated into external CSS (portable and clean)
- Font and colors locked to system design spec
- No inline style or duplicated fields
