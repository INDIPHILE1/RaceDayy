# RaceDayy — Event Management System (Part 3)

## Overview
RaceDayy is a full-stack event management system designed for the South African road running, walking, and cycling community. This repository contains the *Part 3 implementation*, featuring an ASP.NET Core 8.0 MVC web application integrated with Azure Blob Storage for cloud image uploads and fully containerized using Docker.

## Features
- *Role-Based Access:* Distinct interfaces and permissions for Admin, Organizer, and Participant.
- *Event Management:* Organizers can Create, Read, Update, and Delete events, including uploading event banners.
- *Cloud Integration:* Azure Blob Storage is used to securely host and serve event banner images.
- *Enrolments:* Participants can browse events, view categories, and securely enroll.
- *Modern UI:* A responsive, energetic sporting theme utilizing a custom Purple, Blue, and Grey color palette with Bootstrap 5. Enrolment statuses are visually distinct (e.g., Green for Registered, Amber for Pending).
- *Containerization:* The application is fully containerized using Docker for consistent deployment.
- *Unit Testing:* Comprehensive xUnit tests covering controllers and logic.

## Technologies Used
- ASP.NET Core 8.0 (MVC)
- Entity Framework Core (Code-First)
- SQL Server
- ASP.NET Core Identity
- Azure Blob Storage (Azure.Storage.Blobs)
- xUnit & Moq for Unit Testing
- Docker
- GitHub Actions (CI/CD)

## Setup Instructions (Local)

### Prerequisites
- Visual Studio 2022
- .NET 8.0 SDK
- SQL Server (Express or Developer edition)

### Running the Project
1. Clone the repository.
2. Open RaceDayy.sln in Visual Studio.
3. Ensure the appsettings.json connection string points to your local SQL Server.
4. (Optional) Add your Azure Connection String to your local User Secrets to test image uploads.
5. Open the Package Manager Console and run: Update-Database
6. Press *F5* to run the project.

### Default Seeded Users
| Role | Email | Password |
|---|---|---|
| Admin | admin@admin.com | Admin1@ |

## 🐳 Docker Instructions

The application can be run inside a Docker container using the following commands:

1. *Build the Docker image:*
   ```bash
   docker build -t racedayy-app .
: Run the container:

bash
docker run -d -p 8080:8080 --name racedayy-container racedayy-app
Access the application:
Open your browser and navigate to http://localhost:8080.

CI/CD Status
GitHub Actions is configured to automatically build the project and run all unit tests on every push to the master branch.
### GITHUB WORKFLOW ACTIONS

<img width="1580" height="437" alt="image" src="https://github.com/user-attachments/assets/30b93cb3-3df6-4e94-837a-8a560d3f0b68" />

<img width="1427" height="477" alt="image" src="https://github.com/user-attachments/assets/0a4ab485-263e-4cb7-a514-5b2d49002462" />


Video Walkthrough
[Watch the Part 3 walkthrough here](https://youtu.be/OmEuaEb_98o)

Author
Student Number: ST10459365

Module: PROG6212

Institution: Rosebank International University
