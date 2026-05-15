# FounderFlow 🚀

**FounderFlow** is a production-grade SaaS platform designed for startup founders and investors. it provides a comprehensive suite of tools for financial management, expense tracking, and funding lifecycle management.

[![Tech Stack](https://img.shields.io/badge/Stack-React%20%7C%20Laravel%20%7C%20PostgreSQL-blue)](https://github.com/shakshii2004/FounderFlow)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)

---

## ✨ Key Features

### 📊 For Founders
- **Financial Dashboard**: Track burn rate, runway, and growth metrics in real-time.
- **Expense & Revenue Tracking**: Detailed categorization and recurring entry management.
- **Funding Lifecycle**: Create and manage funding requests with pitch details and equity offers.
- **Analytics & Reporting**: Generate professional PDF/CSV financial reports.

### 💼 For Investors
- **Startup Discovery**: Search and filter startups by industry, stage, and valuation.
- **Deep Analytics**: Access detailed financial health metrics for potential investments.
- **Interest Pipeline**: Signal interest and track your investment pipeline.

### 🛡️ Platform Security
- **Role-Based Access Control (RBAC)**: Distinct permissions for Founders, Investors, and Admins.
- **Secure Authentication**: Laravel Sanctum with httpOnly cookie support.
- **Data Integrity**: Comprehensive validation and audit logging.

---

## 🛠️ Technology Stack

| Layer | Technology |
| :--- | :--- |
| **Frontend** | React, Vite, TypeScript, Tailwind CSS, Zustand, Recharts |
| **Backend** | Laravel 12, PHP 8.x, PostgreSQL |
| **Auth** | Laravel Sanctum |
| **Cache/Queue** | Redis, Laravel Queues |
| **Infrastructure** | Docker, Docker Compose |

---

## 📂 Project Structure

The project follows a clean, decoupled architecture:

```txt
founderflow/
├── frontend/   # React + Vite + TypeScript
├── backend/    # Laravel 12 API
├── docker/     # Infrastructure configuration
└── PROMPTS/    # Design & development guidelines
```

---

## 🚀 Getting Started

### Prerequisites
- Docker & Docker Compose
- Node.js (for local frontend dev)
- PHP 8.2+ (for local backend dev)

### Quick Start with Docker

1. **Clone the repository**
   ```bash
   git clone https://github.com/shakshii2004/FounderFlow.git
   cd FounderFlow
   ```

2. **Initialize Environment**
   ```bash
   cp backend/.env.example backend/.env
   cp frontend/.env.example frontend/.env
   ```

3. **Spin up Services**
   ```bash
   docker-compose up -d --build
   ```

4. **Run Migrations & Seeders**
   ```bash
   docker-compose exec backend php artisan migrate --seed
   ```

The applications will be available at:
- **Frontend**: `http://localhost:5173`
- **Backend API**: `http://localhost:8000`

---

## 📖 Documentation
Detailed documentation for specific components:
- [Architecture Overview](ARCHITECTURE.md)
- [API Contracts](API_CONTRACTS.md)
- [Database Schema](DB_SCHEMA.md)
- [Project Roadmap](ROADMAP.md)

---

## 📄 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
