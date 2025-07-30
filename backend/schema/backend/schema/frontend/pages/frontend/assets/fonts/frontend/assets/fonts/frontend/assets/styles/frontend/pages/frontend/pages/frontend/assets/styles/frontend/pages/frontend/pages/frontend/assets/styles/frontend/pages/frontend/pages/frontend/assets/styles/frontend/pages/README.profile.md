# Ebed Profile Page Overview

## 🧱 Structure
- `profile.html` — Profile view/edit page for logged-in users
- `../assets/fonts/kanit.css` — Locked Kanit font
- `../assets/fonts/logo-font.css` — System name styling
- `../assets/styles/profile.css` — UI styling matching login/register/reset pages

## 📋 Field Rationale
- **Username** — Display-only (disabled); audit-linked identifier, not editable
- **Full Name** — Editable user metadata
- **Email** — Editable field for contact or notifications

## 🎨 Design Tokens
- **Background**: `#F5F5DC` (Beige)
- **Text**: `#333333` (Dark gray)
- **Primary Button**: `#3D4C5A` (Blue-gray)
- **Font**: Kanit (locked)

## ✅ Audit Notes
- `username` is locked for integrity; matches user schema logic
- No role/status editing on this page
- Layout and styles follow system-wide locked UI standard
- All styles and assets loaded via relative paths (portable and auditable)
