# AQC Account Ledger Software & Property Flow Design

This repository contains two complete projects: **Account Ledger Software** (Backend) and **Property Flow Design** (Frontend) for AQC Company's commission management system.

## 🏗️ Project Structure

```
├── Account-Ledger-Software/     # Backend Node.js + Supabase
├── property-flow-design/         # Frontend React + TypeScript
└── README.md                     # This file
```

## 🚀 Account Ledger Software (Backend)

A comprehensive Node.js backend application for managing AQC Company's commission-based financial transactions.

### ✨ Features

- **AQC Waterfall Commission Flow**: 3% commission from clients, 1% incentive to vendors
- **Party Management**: Create and manage clients/vendors with commission structures
- **Ledger Management**: Track Credit/Debit transactions with running balances
- **Monday Final Settlement**: Weekly transaction settlement system
- **Authentication**: JWT + Google OAuth integration
- **Database**: Supabase (PostgreSQL) with Row Level Security

### 🛠️ Tech Stack

- **Runtime**: Node.js + Express.js
- **Database**: Supabase (PostgreSQL)
- **Authentication**: JWT, Google OAuth
- **Security**: Helmet, CORS, Rate Limiting
- **Validation**: Input validation and sanitization

### 📁 Key Components

- **Controllers**: Business logic for all operations
- **Models**: Database interaction layer
- **Routes**: API endpoint definitions
- **Middleware**: Authentication and validation
- **Scripts**: Database setup and maintenance utilities

### 🔧 Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/Aadarsh2021/Rough.git
   cd Rough/Account-Ledger-Software
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Configure environment**
   - Copy `.env.example` to `.env`
   - Add your Supabase credentials
   - Configure Google OAuth

4. **Setup database**
   ```bash
   npm run setup-db
   ```

5. **Start the server**
   ```bash
   npm start
   ```

## 🎨 Property Flow Design (Frontend)

A modern React frontend application for the Account Ledger Software with beautiful UI/UX.

### ✨ Features

- **Dashboard**: Financial overview with commission metrics
- **Party Management**: Create and edit client/vendor records
- **Ledger View**: Individual party transaction history
- **Monday Final**: Settlement process interface
- **Responsive Design**: Mobile-first approach
- **Real-time Updates**: Live data synchronization

### 🛠️ Tech Stack

- **Framework**: React 18 + TypeScript
- **Build Tool**: Vite
- **Styling**: Tailwind CSS + Shadcn UI
- **State Management**: React Hooks + Context
- **Authentication**: Firebase + Google Auth
- **API**: Axios for backend communication

### 📁 Key Components

- **Pages**: Main application views
- **Components**: Reusable UI components
- **Contexts**: Authentication and state management
- **Hooks**: Custom React hooks
- **Types**: TypeScript type definitions

### 🔧 Setup Instructions

1. **Navigate to frontend directory**
   ```bash
   cd property-flow-design
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Configure environment**
   - Copy `.env.example` to `.env`
   - Add your Firebase configuration
   - Set backend API URL

4. **Start development server**
   ```bash
   npm run dev
   ```

## 🔄 AQC Commission Flow

### 💰 Business Logic

1. **Client Transaction**: Client pays amount to AQC
2. **AQC Commission**: AQC takes 3% commission
3. **Vendor Payment**: AQC pays remaining amount to vendor
4. **Vendor Incentive**: AQC gives 1% incentive to vendor

### 📊 Example Transaction

- **Original Amount**: ₹100,000
- **AQC Commission (3%)**: ₹3,000
- **Vendor Receives**: ₹97,000
- **Vendor Incentive (1%)**: ₹1,000
- **AQC Net Profit**: ₹2,000

## 🚀 Deployment

### Backend (Render)
- Configured with `render.yaml`
- Automatic deployment from GitHub
- Environment variables management

### Frontend (Vercel)
- Configured with `vercel.json`
- Automatic deployment from GitHub
- Environment variables management

## 📚 Documentation

- **Backend**: See `Account-Ledger-Software/README.md`
- **Frontend**: See `property-flow-design/README.md`
- **Database**: See `Account-Ledger-Software/supabase-schema.sql`
- **API**: See individual route files

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## 📄 License

This project is proprietary software for AQC Company.

## 👥 Team

- **Backend Development**: Node.js + Supabase
- **Frontend Development**: React + TypeScript
- **Business Logic**: AQC Commission Flow
- **Database Design**: PostgreSQL with RLS

## 🔗 Links

- **Repository**: [https://github.com/Aadarsh2021/Rough](https://github.com/Aadarsh2021/Rough)
- **Backend API**: [https://account-ledger-software.onrender.com](https://account-ledger-software.onrender.com)
- **Frontend**: [Deployed on Vercel]

---

**Built with ❤️ for AQC Company's Commission Management System**
