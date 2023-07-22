# DoctorAPP Project 

## Frameworks and Language Used

<p align="center">
<a href="Java url">
    <img alt="Java" src="https://img.shields.io/badge/Java->=8-darkblue.svg" />
</a>
  <a href="Spring Boot url" >
    <img alt="Spring Boot" src="https://img.shields.io/badge/Spring Boot-3.0.6-brightgreen.svg" />
</a>
<a href="Maven url" >
    <img alt="Maven" src="https://img.shields.io/badge/maven-3.0.5-brightgreen.svg" />
</a>
  
<a >
    <img alt="MySQL" src="https://img.shields.io/badge/MySQL-blue.svg">
</a>
</p>

The DoctorAPP is developed using the Spring Framework, specifically Spring Boot, for building the backend of the application. The primary language used for development is Java.

## Data Flow

### 1. AppointmentController
The `AppointmentController` class handles incoming HTTP requests related to appointments and directs them to the appropriate service methods.

- `getAllAppointments()`: This endpoint responds to a GET request to "/appointments" and returns a list of all appointments available in the application.

### 2. DoctorController
The `DoctorController` class handles incoming HTTP requests related to doctors and directs them to the appropriate service methods.

- `addDoctor()`: This endpoint responds to a POST request to "/doctor" and adds a new Doctor object to the application based on the provided JSON data in the request body.

- `getAllDoctors()`: This endpoint responds to a GET request to "/doctors" and returns a list of all doctors available in the application.

### 3. PatientController
The `PatientController` class handles incoming HTTP requests related to patients and directs them to the appropriate service methods.

- `signUpPatient()`: This endpoint responds to a POST request to "/patient/signup" and signs up a new patient based on the provided patient data in the request body.

- `signInPatient()`: This endpoint responds to a POST request to "/patient/signIn" and handles patient sign-in using the provided credentials.

- `sigOutPatient()`: This endpoint responds to a DELETE request to "/patient/signOut" and signs out a patient based on the provided email and token in the request.

- `getAllPatients()`: This endpoint responds to a GET request to "/patients" and returns a list of all patients available in the application.

- `scheduleAppointment()`: This endpoint responds to a POST request to "/appointment/schedule" and schedules a new appointment for a patient based on the provided appointment data, email, and token in the request.

- `cancelAppointment()`: This endpoint responds to a DELETE request to "/appointment/cancel" and cancels an appointment for a patient based on the provided email and token in the request.

### 4. Repository
The repository layer is not explicitly shown in this code snippet, but it would typically be implemented using Spring Data JPA or any other data access technology. It manages the interactions with the underlying database and provides methods for CRUD operations on the entities.

## Data Structure Used in Your Project

The primary data structures used in the DoctorAPP project are `Doctor`, `Patient`, `Appointment`, `SignInInput`, and `SignUpOutput` classes, representing various entities and data transfer objects. These objects are managed and manipulated in lists and collections as needed.

## Project Summary

The DoctorAPP is a backend application built using the Spring Framework with Java as the primary programming language. It provides various endpoints to manage doctors, patients, and appointments. Patients can sign up, sign in, and schedule or cancel appointments. Doctors can be added to the system, and appointments can be viewed. The project follows a structured data flow pattern, with controllers handling incoming requests, services implementing business logic, and a repository for data access to interact with the underlying database.

## Author

👤 **Mohammad Ashif**

* GitHub: [Mohammad Ashif]( https://github.com/ashifdeveloper)

    
---

## 🤝 Contributing

Contributions, issues and feature requests are welcome.
    
---
    
## Show your support

Give a ⭐️ if this project helped you!
    
---
    
## 📝 License

Copyright © 2023 [Mohammad Ashif]( https://github.com/ashifdeveloper).<br />
    
---
