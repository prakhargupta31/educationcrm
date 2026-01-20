🎓 Education CRM System

Java | Spring Boot | Hibernate | MySQL | REST APIs | Thymeleaf

A comprehensive Education CRM System developed using Spring Boot and MySQL, featuring role-based workflows, inquiry tracking, follow-ups, employee sales tracking, orders/enrollments, dashboards, and a complete admin & user UI using Thymeleaf.

This project demonstrates enterprise-level backend architecture, database design, and MVC-based web application development.

🚀 Key Features
🔐 Authentication & User Management

Secure login system

User and employee role handling

Profile management

📝 Inquiry Management

Create and manage student inquiries

Inquiry assignment and tracking

Inquiry-to-order conversion

🔁 Follow-Ups

Scheduled follow-ups for inquiries

Status tracking and reminders

📚 Course Management

Add, update, delete courses

Course assignment and enrollment tracking

📦 Orders / Enrollments

Student enrollments (orders)

Employee-wise order tracking

Sales performance insights

👨‍💼 Employee & Sales Tracking

Employee management

Employee orders & sales information

Sales dashboards & charts

🗣️ Feedback System

Customer feedback collection

Feedback management for admins

📊 Dashboards & Analytics

Orders charts

Employee sales insights

Inquiry & conversion tracking

🌐 REST APIs + MVC

REST APIs for core modules

Thymeleaf-based UI for admin & users

Clean separation of API and MVC layers

🛠️ Tech Stack
Technology	      Purpose
Java	Backend     development
Spring Boot	     Application framework
Spring MVC	      Web layer
Spring Data JPA	 ORM
Hibernate	JPA    implementation
MySQL	Relational database
Thymeleaf	       Server-side UI
HTML / CSS	      Frontend
Maven	Dependency management

🧩 Project Architecture
Client (Browser)
   ↓
Thymeleaf Views / REST Client
   ↓
Controllers
   ↓
Services
   ↓
Repositories (JPA)
   ↓
MySQL Database

📂 Project Structure

src/main/java/in/sp/main
│
├── controllers
│   ├── AdminController
│   ├── CourseController
│   ├── CustomerController
│   ├── EmployeeController
│   ├── InquiryController
│   ├── FollowUpsController
│   ├── OrdersController
│   ├── FeedbackController
│   └── UserController
│
├── services
│   ├── CourseService
│   ├── InquiryService
│   ├── FollowUpsService
│   ├── OrdersService
│   ├── EmployeeService
│   ├── FeedbackService
│   └── UserService
│
├── repositories
│   ├── CourseRepository
│   ├── CustomerRepository
│   ├── EmployeeRepository
│   ├── EmpSalesInfoRepository
│   ├── EmployeeOrdersRepository
│   ├── InquiryRepository
│   ├── FollowUpsRepository
│   ├── OrdersRepository
│   ├── OrdersChartRepository
│   ├── FeedbackRepository
│   └── UserRepository
│
├── entities
│   ├── User
│   ├── Employee
│   ├── Course
│   ├── Inquiry
│   ├── FollowUps
│   ├── Orders
│   ├── Feedback
│   └── BannedUsers
│
├── dto
│   └── PurchasedCourse
│
└── EducationCrmProjectApplication.java

src/main/resources/templates
│
├── login.html
├── index.html
├── admin-login.html
├── inquiry-management.html
├── follow-ups.html
├── course-management.html
├── employee-management.html
├── customer-management.html
├── sales.html
├── user-courses.html
├── user-profile.html
├── provide-feedback.html
├── view-feedbacks.html
├── register.html
└── fragments/

src/main/resources/static
├── css
├── images
└── uploads

=> Setup Steps

Clone repository

git clone https://github.com/your-username/education-crm-system.git


Configure database (application.properties)

spring.datasource.url=jdbc:mysql://localhost:3306/education_crm
spring.datasource.username=root
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update


Run application

mvn spring-boot:run


Open in browser

http://localhost:8080
