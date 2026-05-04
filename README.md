# 🏥 QFlow - Smart Healthcare Token System

![Qflow Hospital Banner](./qflow_hospital_banner_1777821419536.png)

**QFlow** is a modern, premium healthcare management platform designed to eliminate waiting area congestion. It features a real-time patient queue system, event-driven background processing, and a sleek, responsive dashboard for hospital administrators.

---

## 🚀 Key Technological Highlights

### ⚡ Real-Time Queue Management (Socket.io)
Engineered a centralized token system that allows patients to track live queue statuses in real-time.
*   **Instant Updates**: Token updates and "Serve Next" actions are broadcasted immediately via **Socket.io**.
*   **Congestion Control**: Minimizes physical waiting times by allowing remote status tracking.

### 📨 Event-Driven Backend (RabbitMQ)
The system architecture implements an asynchronous message queue using **RabbitMQ** for high scalability.
*   **Automated Reminders**: Appointment reminders and background notification processing are offloaded to background workers.
*   **Reliable Delivery**: Ensures critical healthcare alerts are delivered even during high-traffic bursts.

### 🔐 Secure Multi-Layer Auth
*   **Email & OTP**: Secure account activation and multi-factor verification.
*   **Google OAuth**: Seamless enterprise integration for hospital staff.
*   **Biometric-Ready**: Designed for secure mobile access.

---

## 🛠️ Tech Stack

*   **Frontend**: React 19 + React Router 7
*   **Build Tool**: Vite 8 (Lightning-fast HMR)
*   **Backend**: Node.js + Express + MongoDB
*   **Messaging**: RabbitMQ (AMQP Broker)
*   **Real-time**: Socket.io
*   **Styling**: Premium Vanilla CSS3 (Custom Design System)
*   **Infrastructure**: AWS (S3 Hosting + CloudFront CDN)
*   **CI/CD**: GitHub Actions

---

## 🏗️ System Architecture

QFlow follows a modern decoupled architecture:
1.  **Patient App (Flutter)**: Mobile interface for patients to book tokens and track status.
2.  **Hospital Dashboard (React)**: The administrative control hub for doctors and staff (this repository).
3.  **Core API (Node.js)**: Central logic engine managing tokens, appointments, and notifications.
4.  **DevOps**: Docker-containerized services with automated deployment pipelines.

---

## 📂 Project Structure

```text
src/
├── components/     # Reusable UI components (Glassmorphic Cards, Premium Buttons)
├── context/        # Global state (AuthContext, QueueState)
├── pages/          # Page-level components (Auth, Dashboard, Profile)
├── services/       # API integration (Axios instance, WebSocket hooks)
└── assets/         # Static images and branding
```

---

## ⚙️ Getting Started

### Prerequisites
*   Node.js (v20+)
*   API Base URL configured in `.env`

### Installation
1.  **Clone the repo**:
    ```bash
    git clone https://github.com/nidhin29/qflow_website.git
    cd qflow_website
    ```
2.  **Install dependencies**:
    ```bash
    npm install
    ```
3.  **Run Development Server**:
    ```bash
    npm run dev
    ```

---

## 🚢 Deployment

The project is automatically deployed to **AWS S3** and **CloudFront** via **GitHub Actions** on every push to the `main` branch, ensuring a zero-downtime update cycle.

---

## 📄 License

This project is private and intended for hospital internal use.

---

*Developed with ❤️ by [Nidhin V Ninan](https://github.com/nidhin29)*
