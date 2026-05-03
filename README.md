# Qflow Hospital Dashboard

![Qflow Hospital Banner](./qflow_hospital_banner_1777821419536.png)

Qflow Hospital is a modern, premium healthcare management platform designed to streamline patient and hospital interactions. This repository contains the front-end dashboard built with React and Vite, featuring a secure authentication system, real-time updates, and a sleek, responsive user interface.

[![React](https://img.shields.io/badge/React-19.0-61DAFB?logo=react&logoColor=black)](https://reactjs.org/)
[![Vite](https://img.shields.io/badge/Vite-6.0-646CFF?logo=vite&logoColor=white)](https://vitejs.dev/)
[![AWS S3](https://img.shields.io/badge/AWS-S3-569A31?logo=amazons3&logoColor=white)](https://aws.amazon.com/s3/)
[![CloudFront](https://img.shields.io/badge/AWS-CloudFront-FF9900?logo=amazon-aws&logoColor=white)](https://aws.amazon.com/cloudfront/)
[![GitHub Actions](https://img.shields.io/badge/CI/CD-GitHub_Actions-2088FF?logo=github-actions&logoColor=white)](https://github.com/features/actions)

---

## 🚀 Key Features

- **🔐 Secure Authentication**: Multi-layered auth flow including:
  - Email/Password Login & Registration.
  - 📧 OTP Verification for secure account activation.
  - 🔑 Password Recovery (Forgot/Reset Password).
  - 🌐 Google OAuth Integration for seamless sign-in.
- **📊 Dynamic Dashboard**: A premium, mesh-gradient powered dashboard for monitoring hospital activities.
- **👤 User Profile Management**: Comprehensive profile settings and account details management.
- **🎨 Premium UI/UX**: Built with Vanilla CSS for maximum performance and flexibility, featuring glassmorphism effects and smooth transitions.
- **📱 Fully Responsive**: Optimized for all screen sizes, from mobile to ultra-wide monitors.
- **⚡ High Performance**: Powered by Vite for lightning-fast HMR and optimized production builds.

---

## 🛠️ Tech Stack

- **Frontend**: React 19, React Router 7
- **Build Tool**: Vite 8
- **Authentication**: Google OAuth 2.0, JWT-based custom auth
- **Styling**: Vanilla CSS3 (Custom Design System)
- **Deployment**: AWS S3 (Static Hosting) + Amazon CloudFront (CDN)
- **CI/CD**: GitHub Actions

---

## 📂 Project Structure

```text
src/
├── components/     # Reusable UI components
│   └── layout/     # Navigation and Layout wrappers
├── context/        # Global state (AuthContext)
├── pages/          # Page-level components
│   ├── Auth/       # Login, Register, OTP, Password Recovery
│   ├── Dashboard/  # Main application dashboard
│   └── Profile/    # User settings and profile
├── services/       # API integration and external services
└── assets/         # Static images and icons
```

---

## ⚙️ Getting Started

### Prerequisites

- Node.js (v20 or higher)
- npm or yarn

### Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/nidhin29/qflow_website.git
   cd qflow_website
   ```

2. **Install dependencies**:
   ```bash
   npm install
   ```

3. **Configure Environment Variables**:
   Create a `.env` file in the root directory:
   ```env
   VITE_GOOGLE_CLIENT_ID=your_google_client_id
   VITE_API_URL=your_backend_api_url
   ```

4. **Run development server**:
   ```bash
   npm run dev
   ```

---

## 🚢 Deployment

The project is automatically deployed to AWS using **GitHub Actions**.

### CI/CD Pipeline
- **Branch**: `main`
- **Build**: Vite production build
- **Storage**: AWS S3 Bucket
- **CDN**: Amazon CloudFront (with automatic cache invalidation)

To deploy, simply push your changes to the `main` branch.

---

## 📄 License

This project is private and intended for Qflow Hospital internal use.

---

*Developed with ❤️ by [Nidhin V Ninan](https://github.com/nidhin29)*
