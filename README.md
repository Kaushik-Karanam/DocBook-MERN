# 🌐 DocBook | Full-Stack Healthcare Platform

DocBook is a robust MERN-stack application designed to bridge the gap between patients and healthcare providers. It features a secure, role-based scheduling system, real-time appointment management, and a centralized dashboard for medical professionals.

![Homepage](./Hook.png)

---

## 🚀 Key Engineering Highlights

- **Role-Based Access Control (RBAC):** Built a secure authentication system with separate registration flows and permissions for Patients and Doctors using JWT.
- **Dynamic Scheduling Engine:** Engineered custom calendar logic to track real-time slot availability, preventing double-bookings and managing practitioner schedules.
- **Cloud Media Integration:** Integrated the **Cloudinary API** to handle high-resolution profile image uploads and secure storage for healthcare professionals.
- **Centralized State Management:** Leveraged **Redux** to synchronize the appointment booking lifecycle across the frontend, ensuring UI consistency during complex data fetches.

---

## 🛠 Tech Stack

![Tech Stack](./Tools.png)

| Layer      | Technology                              |
|------------|-----------------------------------------|
| Frontend   | React.js, Redux, Bootstrap              |
| Backend    | Node.js, Express.js (RESTful API)       |
| Database   | MongoDB (Scalable NoSQL Storage)        |
| Cloud      | Cloudinary (Media Management)           |

---

## 📅 Advanced Scheduling Logic

![Calendar Logic](./Logic.png)

Implementation of the dynamic availability engine. The system calculates open slots in real-time, allowing users to book appointments based on specific doctor schedules.

## 🔄 Appointment Workflow

![Booking Workflow](./Result.png)

A seamless end-to-end flow from doctor discovery to confirmed booking, ensuring data integrity across the MongoDB database.

---

## ⚙️ Getting Started

### Prerequisites

- **Node.js** v16.0.0+
- **npm** v8.0.0+

### Installation & Setup

**1. Clone the Repository**
```bash
git clone https://github.com/Kaushik-Karanam/Docbook.git
cd Docbook
```

**2. Configure Environment Variables**

Create a `.env` file inside the `/server` directory:
```env
SERVER_PORT=5000
MONGO_CONNECTION=your_mongodb_uri
CLOUD_NAME=your_cloudinary_name
API_KEY=your_api_key
API_SECRET=your_api_secret
```

**3. Install Dependencies**

Run the following in both the `/server` and `/client` directories:
```bash
npm install
```

**4. Run the Application**
```bash
# In /server
npm start

# In /client (separate terminal)
npm start
```

The app will be available at `http://localhost:3000`.