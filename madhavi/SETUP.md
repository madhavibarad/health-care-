# Quick Setup Guide

## Prerequisites
- Node.js (v14 or higher)
- npm or yarn

## Installation Steps

1. **Install all dependencies:**
   ```bash
   npm run install-all
   ```
   This will install dependencies for:
   - Root project
   - Backend server
   - React frontend

2. **Start the application:**
   ```bash
   npm run dev
   ```
   This starts both the backend (port 5000) and frontend (port 3000) simultaneously.

   Or start them separately:
   ```bash
   # Terminal 1 - Backend
   npm run server
   
   # Terminal 2 - Frontend
   npm run client
   ```

3. **Access the application:**
   - Frontend: http://localhost:3000
   - Backend API: http://localhost:5000

## First Time Setup

If you encounter any issues:

1. Make sure all dependencies are installed:
   ```bash
   cd server && npm install
   cd ../client && npm install
   ```

2. If port 3000 or 5000 is already in use, you can:
   - Change the port in `client/package.json` scripts
   - Change PORT in `server/index.js`

## Features to Test

1. **Home Page**: Beautiful landing page with service overview
2. **Health Records**: Add and manage medical records
3. **Appointments**: Book doctor appointments or lab tests
4. **Medicine**: Browse and order medicines
5. **Emergency**: Access emergency services
6. **Reports**: Upload and view lab reports

## Troubleshooting

- **Module not found errors**: Run `npm install` in the respective directory
- **Port already in use**: Kill the process using the port or change the port number
- **CORS errors**: Make sure the backend is running on port 5000

Enjoy using Medic! 🏥

