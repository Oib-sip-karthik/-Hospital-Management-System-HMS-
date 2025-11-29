# -Hospital-Management-System-HMS-
A full-stack backend API for managing patients, doctors, appointments, medical records, and billing within a hospital or clinic. This system helps streamline hospital workflows by securely storing, processing, and retrieving healthcare data.  🚀 Features
Hospital Management System (HMS)

A full-stack backend API for managing patients, doctors, appointments, medical records, and billing within a hospital or clinic.
This system helps streamline hospital workflows by securely storing, processing, and retrieving healthcare data.

🚀 Features
👨‍⚕️ Doctor Management

Add, update, delete doctor records

Specialization, experience, availability

Filter doctors by department or specialization

🧑‍🦱 Patient Management

Store and update patient details

Track medical history, prescriptions, lab results

Unique patient ID generation

📅 Appointment Scheduling

Book, reschedule, cancel appointments

Doctor-wise calendar

Prevents double-booking

📑 Medical Records

Store diagnoses, treatment notes, medications

Attach lab reports, files (optional)

Maintain patient visit history

💵 Billing Module

Auto-generate invoices

Consultation + treatment + lab charges

Payment status tracking

🔐 Role-based Authentication (optional)

Admin

Doctor

Receptionist

🧱 Tech Stack

Node.js + Express.js

MongoDB + Mongoose

JWT Authentication (optional)

BCrypt for password encryption

CORS, dotenv, morgan

📁 Folder Structure
hospital-management-system/
│── config/
│   └── db.js
│── models/
│   ├── Doctor.js
│   ├── Patient.js
│   ├── Appointment.js
│   ├── MedicalRecord.js
│   └── Bill.js
│── routes/
│   ├── doctorRoutes.js
│   ├── patientRoutes.js
│   ├── appointmentRoutes.js
│   ├── recordRoutes.js
│   └── billingRoutes.js
│── middleware/
│   └── auth.js
│── server.js
│── package.json
│── .env (ignored)
└── README.md

🔧 Installation & Setup
1️⃣ Clone the repository
git clone https://github.com/<your-username>/hospital-management-system.git
cd hospital-management-system

2️⃣ Install dependencies
npm install

3️⃣ Create .env file
MONGO_URI=your_mongo_connection_string
JWT_SECRET=your_secret
PORT=5000

4️⃣ Start the server
Development:
npm run dev

Production:
npm start


Server runs on:

http://localhost:5000

🔌 API Endpoints
👨‍⚕️ Doctor APIs
Method	Endpoint	Description
POST	/api/doctors	Add a doctor
GET	/api/doctors	Get all doctors
GET	/api/doctors/:id	Get doctor by ID
PUT	/api/doctors/:id	Update doctor
DELETE	/api/doctors/:id	Delete doctor
🧑‍🦱 Patient APIs
Method	Endpoint	Description
POST	/api/patients	Add patient
GET	/api/patients	All patients
GET	/api/patients/:id	Patient details
PUT	/api/patients/:id	Update patient
DELETE	/api/patients/:id	Delete patient
📅 Appointment APIs
Method	Endpoint	Description
POST	/api/appointments	Book appointment
GET	/api/appointments	All appointments
GET	/api/appointments/:id	Appointment details
PUT	/api/appointments/:id	Reschedule
DELETE	/api/appointments/:id	Cancel
📑 Medical Records APIs
Method	Endpoint	Description
POST	/api/records	Add medical record
GET	/api/records/:patientId	Get patient history
PUT	/api/records/:id	Update record
💵 Billing APIs
Method	Endpoint	Description
POST	/api/bills	Create invoice
GET	/api/bills/:patientId	Get bills for a patient
PUT	/api/bills/:id	Update payment status
🧪 Testing

You can test the APIs using:

Postman

Thunder Client (VS Code)

cURL

REST Client Extension

🛠 Future Enhancements

Nurse management

Lab management module

File uploads (prescriptions, reports)

Insurance claims system

Appointment reminders (SMS/Email)

Real-time doctor availability (Socket.io)

📜 License

This project is licensed under the MIT License.

👨‍💻 Author

Abhinava Karthik CY
Full Stack Developer • Backend Enthusiast
GitHub: <https://github.com/Oib-sip-karthik>
