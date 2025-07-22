Data Structure for the Smart Clinic Management System:
    Section 1: MySQL Database design (for structured data)
    Section 2: MongoDB Database design (for unstructured data)

****MySQL Database Design ****
Core Tables
    1. admin
    2. patients
    3. doctors
    4. appointments
    5. scheduling/doctor_availability
    6. billing

    ### Table Name: admin
    - userId INT PRIMARY KEY AUTO_INCREMENT,
    - username VARCHAR(50) UNIQUE,
    - password VARCHAR(255),
    - role ENUM

    ### Table Name: patients
    - patientID INT PRIMARY KEY AUTO_INCREMENT,
    - firstname VARCHAR(50)
    - lastname VARCHAR(50)
    - date_of_birth DATE,
    - gender ENUM
    - phone VARCHAR(15)
    - email VARCHAR(100)
    - address TEXT

    ### Table Name: doctors
    - doctorID INT PRIMARY KEY AUTO_INCREMENT
    - firstname VARCHAR(50)
    - lastname VARCHAR(50)
    - specialty VARCHAR(255)
    - phone VARCHAR(15)
    - email VARCHAR(100)

    ### Table Name: appointments
    - id: INT, Primary Key, Auto Increment
    - doctor_id: INT, Foreign Key → doctors(id)
    - patient_id: INT, Foreign Key → patients(id)
    - appointment_time: DATETIME, Not Null
    - status: INT (0 = Scheduled, 1 = Completed, 2 = Cancelled)

    ### Table name: doctor_availability
    - availability_ID INT PRIMARY KEY AUTO_INCREMENT
    - doctor_ID INT, FOREIGN KEY -> doctors(doctorID)
    - available_date DATE
    - starttime TIME
    - endtime TIME

    ### Table Name: billing
    - bill_ID INT PRIMARY KEY AUTO_INCREMENT
    - patient_ID INT, FOREIGN KEY → patients(id)
    - bill_amount DECIMAL(10, 2)
    - issue_date DATE
    - status ENUM

**MongoDB Design**
   Sample Document Schema: prescriptions Collection
{
  "_id": ObjectId("..."),
  "patient": {
    "patientId": ObjectId("..."),
    "name": "John Doe"
  },
  "doctor": {
    "doctorId": ObjectId("..."),
    "name": "Dr. Smith",
    "specialty": "Cardiology"
  },
  "prescribedOn": ISODate("2025-07-22T14:30:00Z"),
  "medications": [
    {
      "name": "Atorvastatin",
      "dosage": "20mg",
      "frequency": "Once daily",
      "duration": "30 days",
      "notes": "Take with food"
    },
    {
      "name": "Aspirin",
      "dosage": "81mg",
      "frequency": "Once daily",
      "duration": "Indefinite",
      "notes": "Preventive dose"
    }
  ],
  "followUpDate": ISODate("2025-08-22T10:00:00Z"),
  "status": "active",
  "notes": "Patient responded well to initial treatment."
}


    
















    
    

