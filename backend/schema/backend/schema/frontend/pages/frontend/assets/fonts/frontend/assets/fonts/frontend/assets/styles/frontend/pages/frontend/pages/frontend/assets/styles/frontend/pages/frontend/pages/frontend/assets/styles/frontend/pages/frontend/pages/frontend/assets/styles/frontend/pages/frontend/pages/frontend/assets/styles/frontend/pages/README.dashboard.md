# Ebed Dashboard Page Overview

## 🧱 Structure
- `dashboard.html` — User landing page after login
- `../assets/fonts/kanit.css` — Locked Kanit font
- `../assets/fonts/logo-font.css` — Styling for system name
- `../assets/styles/dashboard.css` — Layout and menu styles

## 📋 Menu Rationale
- **Profile** — View/edit personal info
- **Reports** — Access system reports (read-only)
- **Admin** — Admin-only functions (role-based access applies)
- **Logs** — View action trail history
- **Logout** — End session securely

## 🎨 Design Tokens
- **Background**: `#F5F5DC` (Beige)
- **Text**: `#333333` (Dark gray)
- **Primary Buttons**: `#3D4C5A` (Blue-gray)
- **Font**: Kanit (locked)

## ✅ Audit Notes
- Menu links match system routes
- No embedded logic; layout is static
- All styles are external and portable
- Role-based visibility logic will be handled separately
