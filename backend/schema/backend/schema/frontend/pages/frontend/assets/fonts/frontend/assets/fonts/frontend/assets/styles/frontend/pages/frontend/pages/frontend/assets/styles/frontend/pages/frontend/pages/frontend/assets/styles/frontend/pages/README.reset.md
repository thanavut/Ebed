# Ebed Reset Password Page Overview

## 🧱 Structure
- `reset-password.html` — UI for requesting password recovery
- `../assets/fonts/kanit.css` — Locked Kanit font
- `../assets/fonts/logo-font.css` — System name styling
- `../assets/styles/reset-password.css` — Consistent design with login/register pages

## 📋 Field Justification
- **Username or Email** — Only necessary field for initiating reset flow
  - No extra data collected
  - Field label kept generic to allow for flexible backend logic

## 🎨 Design Tokens
- **Background**: `#F5F5DC` (Beige)
- **Text**: `#333333` (Dark gray)
- **Primary Button**: `#3D4C5A` (Blue-gray)
- **Font**: Kanit (locked)

## ✅ Audit Notes
- Layout uses same structure as other user-facing pages
- Styles are fully externalized and portable
- No inline styles or redundant fields
- Page supports eventual backend integration without changes to UI
