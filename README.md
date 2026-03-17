# SlickHood User Manual

**SlickHood** is a rental and property management platform designed to streamline interactions between **Landlords**, **Property Managers**, **Tenants**, and other stakeholders such as **Guards** and **Superadmins**.

The platform enables efficient property management, tenant onboarding, and—critically—**flexible, multi-channel payment processing**.

---

## 🚀 Features

### 🏢 Property & User Management
- Multi-role support:
  - Superadmin
  - Landlord
  - Property Manager
  - Tenant
  - Guard
- Property ownership and assignment
- Tenant allocation to units

---

### 💳 Payments

SlickHood supports multiple payment workflows:

#### 1. Mobile Money (M-Pesa)
- Paybill/Till-based payments
- STK Push (push payment requests to tenant phones)
- Integration via Safaricom Daraja API

#### 2. Card Payments (Flutterwave)
- Accept Visa/Mastercard and other supported methods
- Secure payment processing via Flutterwave

#### 3. Manual Payments
- Cash payments
- Bank transfers
- Offline transaction recording by property managers

---

### ⚙️ Payment Configuration

- Landlords configure payment options per profile
- Supports:
  - M-Pesa credentials (Paybill, Consumer Key/Secret, STK Passkey)
  - Flutterwave credentials (Public, Secret, Encryption Keys)
- Configurations are:
  - **Encrypted at rest**
  - **Submitted for verification**
  - **Approved by Superadmin before use**
- Verified payment options can be assigned to properties

---

### 🔐 Security

- Sensitive credentials are encrypted before storage
- Secret keys are never exposed after submission
- Role-based access control across the platform
- Payment configurations undergo verification before activation

---

## 🧩 System Overview

```text
Tenant → Makes Payment → Payment Gateway (M-Pesa / Flutterwave)
        → Platform processes transaction
        → Linked to Property → Landlord/Manager visibility

Manual Flow:
Tenant → Pays Offline → Property Manager Records Payment → System Updates Ledger
