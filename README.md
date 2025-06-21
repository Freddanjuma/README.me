# Airbnb Clone Project

## Project Overview
The **Airbnb Clone Project** is a full-stack web development project designed to replicate the core features of the Airbnb platform. The goal is to build a scalable and responsive application that enables users to view, search, and manage property listings.

### Project Goals
- Implement a full-stack booking platform.
- Practice OOP, RESTful API design, and UI development.
- Develop both frontend and backend systems.
- Enable user registration, property listings, and bookings.

### Tech Stack
- **Frontend:** HTML, CSS, JavaScript
- **Backend:** Python (Django)
- **Database:** PostgreSQL
- **Version Control:** Git and GitHub
- **Deployment:** Docker, GitHub Actions (CI/CD)

---

## Team Roles

### 1. Business Analyst
Gathers business requirements and translates them into technical specifications.

### 2. Product Owner
Sets the product vision and prioritizes features to ensure alignment with business goals.

### 3. Project Manager
Coordinates tasks, schedules, and team communication to ensure timely project delivery.

### 4. UI/UX Designer
Designs intuitive interfaces and user-friendly experiences through wireframes and prototypes.

### 5. Software Architect
Defines system architecture, selects technologies, and enforces coding standards.

### 6. Software Developers
Write and maintain the application’s frontend and backend code.

### 7. QA Engineers
Test the application for bugs and verify it meets functional requirements.

### 8. Test Automation Engineers
Create and maintain automated test scripts to streamline testing efforts.

### 9. DevOps Engineer
Manages CI/CD pipelines, deployments, and infrastructure for stable delivery.

---

## Technology Stack

### Django
A high-level Python web framework used to build the backend and REST APIs.

### PostgreSQL
A powerful, open-source relational database used to store all application data.

### GraphQL (Optional)
Enables flexible and efficient data querying from clients to the server.

### HTML/CSS/JavaScript
Builds the structure, style, and interactivity of the web interface.

### Docker
Used to containerize the application for consistent deployment across environments.

### GitHub Actions
Automates testing, builds, and deployments via CI/CD workflows.

---

## Database Design

### Entities & Fields

#### Users
- `id`, `name`, `email`, `password_hash`, `user_type`  
- A user can list multiple properties and make multiple bookings.

#### Properties
- `id`, `title`, `description`, `location`, `price_per_night`  
- A property belongs to a user and can have many bookings and reviews.

#### Bookings
- `id`, `user_id`, `property_id`, `start_date`, `end_date`  
- Each booking links a user to a property for a date range.

#### Reviews
- `id`, `user_id`, `property_id`, `rating`, `comment`  
- A user can review a property after booking it.

#### Payments
- `id`, `booking_id`, `amount`, `payment_method`, `payment_status`  
- Each payment is associated with one booking.

---

## Feature Breakdown

### User Management
Users can register, log in, manage profiles, and switch between guest and host roles.

### Property Management
Hosts can list properties, including details, pricing, and availability.

### Booking System
Guests can search for properties and make date-specific bookings.

### Payment Integration
Enables users to securely pay for bookings via supported payment methods.

### Search & Filter
Users can filter properties based on price, location, and features.

### Reviews & Ratings
Guests can leave feedback on properties to help others make informed decisions.

### Admin Dashboard (Optional)
Admins can monitor users, bookings, payments, and platform analytics.

---

## API Security

### Authentication
Secured using JWT tokens for user identity verification.

### Authorization
Role-based access control ensures actions match user permissions.

### Data Validation
Input data is validated and sanitized to prevent injection attacks.

### HTTPS and Headers
Secures data in transit and adds protection with security headers.

### Rate Limiting
Prevents abuse by limiting repeated requests to critical endpoints.

### Payment Security
Payment data is handled via PCI-compliant third-party services.

---

## CI/CD Pipeline

CI/CD automates code testing and deployment, ensuring stability and speed in the development process.

### Why It Matters
- Detects issues early through automated testing
- Reduces deployment errors and manual steps
- Speeds up the delivery of new features

### Tools Used
- **GitHub Actions**: Runs tests and deploys code after each commit.
- **Docker**: Packages the app for consistent deployment.
- **Heroku / AWS / Render**: Optional platforms for production hosting.
