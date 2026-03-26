# SecureVendor Africa 🔒
### Secure Peer-to-Peer Student Marketplace for ALU

> Built by **Hirwa Hebert Crispin** — African Leadership University, 2026

---

## What is SecureVendor Africa?

SecureVendor Africa is a security-first web marketplace built exclusively for ALU students. It solves a real problem: students currently use unencrypted platforms like WhatsApp to share sensitive payment details (mobile money numbers, home addresses) when trading — making them vulnerable to fraud and data interception.

SecureVendor moves student commerce to a verified, encrypted, and auditable environment.

---

## Live Demo

🌐 **[View Live App](https://hirwavsopps.github.io/SecureVendor-Africa)**

---

## Features

| Feature | Description | SRS Reference |
|---|---|---|
| 🔐 ALU ID Verification | Only @alustudent.com emails can register as vendors | FR1 |
| 🔑 MFA Login | 6-digit code required for all vendor logins | FR2 |
| 🛍 External Buyer Registration | Non-ALU buyers can register with Gmail/phone | FR3 |
| 💬 E2EE Encrypted Chat | End-to-end encrypted messaging for payment details | FR4 |
| 📸 Secure Product Upload | Vendors list products with verified badges | FR5 |
| 📋 Transaction Log | Immutable audit trail of all trades | FR6 |
| 🚨 Fraud Reporting | One-click report with auto-freeze at 3+ reports | FR7 |
| ⚙️ Admin Panel | User management, audit reports, freeze accounts | Section 2.3 |

---

## Demo Accounts

| Role | Email | Password | MFA Code |
|---|---|---|---|
| Vendor | any@alustudent.com | any (8+ chars) | 123456 |
| Buyer | any@gmail.com | any (8+ chars) | — |
| Admin | admin@alustudent.com | any | 123456 |
| Google Login | Click "Continue with Google" | — | 123456 |

---

## How to Run Locally

This is a pure frontend HTML application — no installation required.

### Option 1: Open directly
```bash
# Clone the repository
git clone https://github.com/Hirwavsopps/SecureVendor-Africa.git

# Navigate into the folder
cd SecureVendor-Africa

# Open in browser
open index.html
# OR double-click index.html in your file explorer
```

### Option 2: Use Live Server (recommended)
```bash
# Install VS Code Live Server extension, then:
# Right-click index.html → Open with Live Server
```

### Requirements
- Any modern web browser (Chrome, Edge, Safari, Firefox)
- No Node.js, no npm, no database setup needed
- Internet connection (for Google Fonts only)

---

## Project Structure

```
SecureVendor-Africa/
│
├── index.html          # Complete single-page application
└── README.md           # This file
```

---

## How to Use the App

1. **Landing Page** — Overview of features, click "Get Started"
2. **Register** — Choose Vendor or Buyer role, fill in details
3. **MFA** — Enter code `123456` (vendors only)
4. **Dashboard** — Access all features from the sidebar:
   - **Browse Market** — View all listings with verified badges
   - **Encrypted Chat** — Message vendors securely (E2EE)
   - **Transaction Log** — View immutable audit trail
   - **Report Fraud** — Submit fraud reports
   - **List Product** — (Vendors only) Add new listings
   - **Admin Panel** — (Admin only) Manage users and reports

---

## System Design

Built according to the Software Requirements Specification (SRS) v2.0:

- **Frontend**: HTML5, CSS3, Vanilla JavaScript
- **Authentication**: Simulated Google OAuth 2.0 + MFA flow
- **Encryption**: E2EE chat interface (AES-256 in production)
- **Database**: Client-side state (PostgreSQL in production)
- **Deployment**: GitHub Pages (HTTPS)

---

## SRS Document

📄 [View Full SRS Document](YOUR_SRS_LINK_HERE)

---

## Deployment

Deployed on **GitHub Pages** via HTTPS.

To redeploy:
1. Go to repository Settings → Pages
2. Set source to `main` branch, `/ (root)`
3. Save — site is live at `https://hirwavsopps.github.io/SecureVendor-Africa`

---

*African Leadership University — Introduction to Software Engineering — 2026*
