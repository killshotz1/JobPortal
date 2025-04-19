# JobPortal
a job portal project where people can log in as a user or recruiter 
🧑‍💼 Job Portal Backend (Spring Boot)
This is a Job Portal Web Application backend built using Java + Spring Boot, featuring role-based access control, JWT authentication, and RESTful APIs.

It allows two main roles:

Recruiters: Post job listings

Job Seekers: Search, apply, and view jobs

✨ Features
🔐 Role-based authentication (Recruiter & Seeker)

🛡️ JWT Token-based security

📄 RESTful API architecture

📦 Layered architecture using Controller, Service, Repository

🧪 Tested endpoints with Postman

📚 Proper use of DTOs and models

🔁 Password encryption using BCrypt

🚀 Technologies Used
Java 17

Spring Boot

Spring Security

Spring Data JPA (Hibernate)

H2 / MySQL (configurable)

Lombok

Maven

📁 Project Structure
arduino
Copy
Edit
src
├── controller
├── service
├── repository
├── model
├── dto
├── config
└── util
🔧 How to Run
Clone the repo:

bash
Copy
Edit
git clone https://github.com/your-username/job-portal-backend.git
Open in your favorite IDE (IntelliJ / VS Code)

Set up the database in application.properties (H2 or MySQL)

Run the application:

bash
Copy
Edit
mvn spring-boot:run
Test with Postman or integrate with a frontend.

📌 Endpoints Overview

Method	Endpoint	Access Role	Description
POST	/auth/register	Public	Register user/recruiter
POST	/auth/login	Public	Login and get JWT
POST	/recruiter/postJob	RECRUITER	Post a new job
GET	/seeker/jobs	USER	View all jobs
POST	/seeker/apply/{jobId}	USER	Apply to a job
📌 Future Improvements
Swagger API documentation

Email notifications

Frontend integration (React/Angular)

Job application history

Admin panel

🧑‍💻 Author
Made with 💻 by Aryan – learning Spring Boot and building real-world projects!
