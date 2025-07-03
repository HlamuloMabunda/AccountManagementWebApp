# Account Management API

A web-based Account Management System designed for environments like hospital cafeterias where users (e.g. doctors) can make purchases on account and settle balances monthly. The system integrates with Oracle Simphony POS, providing account creation, sales posting, payment processing, and reporting functionalities.

> Developed by Micros South Africa (Pty) Ltd  
> Reg. 2001/022540/07  
> [micros.co.za](https://micros.co.za)  
> Adapt IT Johannesburg Campus  
> 152, 14th Road, Midrand, 1687  
> 📞 +27 10 494 0000

---

## 🧰 Tech Stack

- **Frontend**: Angular (basic prototype)  
- **Backend**: .NET 6 Web API (VS 2022)  
- **Database**: SQL Server with stored procedures & triggers  
- **Authentication**: Role-based (Identity / JWT-based)  
- **Deployment**: Runs locally on IIS Express or Kestrel (dev)

---

## 🔐 Key Features

### ✅ Account Management

- Create and update user accounts
- Real-time form validation (phone number, limits)
- Role-based access control (admin, cashier, viewer)
- Audit logs of all account changes

### 🛒 Posting Sales (POS Integration)

- WPF UI to link sales with accounts
- API to post transactions and close bills in Simphony
- Handles over-limit errors and retries
- Full data consistency even with Simphony timeouts

### 📊 Transaction Reporting

- Interactive Angular reporting (charts & tables)
- Filters: date range, transaction type, balances
- Export to PDF/CSV
- Caching for frequent report queries

### 💳 Payment Handling

- WPF interface for making full/partial payments
- Instant feedback on transaction success/failure
- Transaction-safe API to prevent duplicates
- Triggers to auto-update account balances on payment

---

---

## 🚀 Getting Started

### 🔧 Requirements

- Visual Studio 2022  
- SQL Server  
- Node.js + Angular CLI (for frontend)  

### 🛠️ Setup

1. **Clone the repo**

```bash
git clone https://github.com/HlamuloMabunda/AccountManagement.API.git
cd AccountManagement.API


