# Doctor Booking Appointment Application

A full-stack web application that allows patients to book appointments with doctors online. Features include user authentication, doctor profiles, appointment scheduling, and availability management.

## Features

- **User Authentication**: Secure registration and login for patients and doctors
- **Doctor Profiles**: View doctor details, specializations, and experience
- **Appointment Booking**: Schedule appointments with available time slots
- **Availability Management**: Doctors can set their working hours and availability
- **Appointment Management**: View, reschedule, and cancel appointments
- **Notifications**: Email and in-app notifications for appointment confirmations
- **Reviews & Ratings**: Patients can rate and review doctors
- **Admin Dashboard**: Manage users, doctors, and appointments

## Tech Stack

### Frontend
- React 18+
- Vite
- Tailwind CSS
- Axios
- React Router
- Redux Toolkit

### Backend
- Node.js
- Express.js
- MongoDB
- Mongoose
- JWT Authentication
- Bcrypt for password hashing

## Project Structure

```
doc1/
├── backend/              # Node.js Express server
│   ├── models/
│   ├── routes/
│   ├── controllers/
│   ├── middleware/
│   ├── config/
│   └── server.js
├── frontend/             # React application
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── redux/
│   │   └── App.jsx
│   └── package.json
└── README.md
```

## Getting Started

### Prerequisites
- Node.js 16+
- MongoDB
- npm or yarn

### Backend Setup

```bash
cd backend
npm install
cp .env.example .env
npm run dev
```

### Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

## API Documentation

Base URL: `http://localhost:5000/api`

### Authentication
- `POST /auth/register` - Register new user
- `POST /auth/login` - User login
- `POST /auth/logout` - User logout

### Doctors
- `GET /doctors` - List all doctors
- `GET /doctors/:id` - Get doctor details
- `PUT /doctors/:id` - Update doctor profile
- `GET /doctors/:id/availability` - Get doctor availability

### Appointments
- `POST /appointments` - Book appointment
- `GET /appointments/:userId` - Get user appointments
- `PUT /appointments/:id` - Update appointment
- `DELETE /appointments/:id` - Cancel appointment

### Reviews
- `POST /reviews` - Add review
- `GET /reviews/:doctorId` - Get doctor reviews

## License

MIT
