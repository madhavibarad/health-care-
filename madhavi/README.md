# Medic - A Unified Digital Healthcare Platform

A comprehensive healthcare platform that brings together all essential healthcare services in one place.

## Features

- **Centralized Health Records**: Securely store and manage all your medical records
- **Appointment & Service Booking**: Book appointments with doctors and schedule lab tests
- **Medicine Ordering**: Order medicines from trusted pharmacies
- **Emergency Services Access**: Quick access to ambulance and emergency services
- **Online Report Delivery**: Receive lab test reports and medical documents online

## Tech Stack

- **Frontend**: React, HTML, CSS, JavaScript
- **Backend**: Node.js, Express
- **Styling**: Modern CSS with gradients and animations

## Installation

1. Install all dependencies:
```bash
npm run install-all
```

2. Start the development server (runs both frontend and backend):
```bash
npm run dev
```

Or start them separately:

**Backend (runs on port 5000):**
```bash
npm run server
```

**Frontend (runs on port 3000):**
```bash
npm run client
```

## Project Structure

```
healthcare/
├── client/          # React frontend application
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   │   ├── Home.js
│   │   │   ├── HealthRecords.js
│   │   │   ├── Appointments.js
│   │   │   ├── MedicineOrder.js
│   │   │   ├── Emergency.js
│   │   │   └── Reports.js
│   │   ├── App.js
│   │   └── index.js
│   └── package.json
├── server/          # Node.js backend API
│   ├── index.js
│   └── package.json
└── package.json
```

## API Endpoints

### Health Records
- `GET /api/health-records` - Get all health records
- `POST /api/health-records` - Create a new health record
- `PUT /api/health-records/:id` - Update a health record
- `DELETE /api/health-records/:id` - Delete a health record

### Appointments
- `GET /api/appointments` - Get all appointments
- `POST /api/appointments` - Book a new appointment
- `PUT /api/appointments/:id` - Update an appointment

### Medicines
- `GET /api/medicines` - Get available medicines
- `POST /api/orders` - Place a medicine order
- `GET /api/orders` - Get all orders

### Reports
- `GET /api/reports` - Get all reports
- `POST /api/reports` - Upload a new report

### Emergency
- `POST /api/emergency` - Submit emergency request

### Doctors & Lab Tests
- `GET /api/doctors` - Get list of doctors
- `GET /api/lab-tests` - Get list of lab tests

## Usage

1. Navigate to `http://localhost:3000` in your browser
2. Use the navigation menu to access different features:
   - **Home**: Overview of all services
   - **Health Records**: Manage your medical records
   - **Appointments**: Book doctor appointments or lab tests
   - **Medicine**: Order medicines online
   - **Reports**: View and upload lab reports
   - **Emergency**: Access emergency services

## Features Overview

### Home Page
- Beautiful hero section with animated cards
- Service overview cards
- Statistics section

### Health Records
- Add, view, and delete health records
- Store diagnosis, medications, and doctor information

### Appointments
- Book doctor appointments
- Schedule lab tests
- View appointment history

### Medicine Order
- Browse available medicines
- Add to cart functionality
- Place orders with delivery details

### Emergency Services
- Quick action buttons for emergency numbers
- Emergency request form
- Important emergency information

### Reports
- Upload lab reports and documents
- View and download reports
- Track medical documents

## Development

The application uses:
- React Router for navigation
- Axios for API calls
- Modern CSS with gradients and animations
- Responsive design for mobile and desktop

## Notes

- The backend uses in-memory storage (data resets on server restart)
- In production, connect to a proper database (MongoDB, PostgreSQL, etc.)
- Add authentication and authorization for production use
- Implement file upload handling for reports in production

## License

ISC

