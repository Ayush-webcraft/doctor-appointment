# DoctorOnCall — Online doctor appointments (Frontend)

**A modern React-based frontend where patients book visits, doctors manage schedules, and admins oversee the clinic system.**

[![Live demo — Netlify](https://img.shields.io/badge/Live_demo-Netlify-00C7B7?logo=netlify)](https://dental-doctor-ujjal.netlify.app/)

---

## Tech Stack & Features

| Layer | Tools |
|-------|--------|
| **Website (frontend)** | React, Redux Toolkit, Ant Design, React Router, Axios |

### Key Features
- **Visitors**: Home, about, services, blog, contact, search and filter doctors.
- **Patients**: Sign up / sign in, dashboard, favourites, appointments, invoices, prescriptions, track appointment with ID.
- **Doctors**: Sign up (with email verification), dashboard, appointments, patients, schedule, prescriptions, reviews, blogs, invoices, profile settings.
- **Admins**: Separate admin area: dashboard stats, manage appointments, doctors, patients, specialties, reviews, transactions.

---

## Project Layout

```
Doctor-Appointment/          ← React app (run from here)
├── public/                  ← Static assets
├── src/                     ← Source code (React components, Redux slices, style configurations)
└── .env                     ← Environment configuration for API endpoint
```

---

## Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/Ujjalzaman/Doctor-Appointment.git
cd Doctor-Appointment
```

### 2. Configure Environment Variables
Create or edit `.env` in the root directory:
```env
REACT_APP_API_BASE_URL=https://your-deployed-backend-api.com
```

### 3. Install & Start
```bash
# Install dependencies
npm install

# Start local development server
npm start
```
Open [http://localhost:3000](http://localhost:3000) to view the application in the browser.

---

## Deployment

This repository includes a pre-configured CI/CD workflow for deploying to an AWS EC2 instance:
- **Workflow Path**: `.github/workflows/frontend-deploy.yml`
- **Action**: Builds the React application and copies the static assets directly to the target directory of your EC2 instance on every push to the `main` branch.
