# RaceDayy — Event Management System (Part 2)

## Overview
RaceDayy is a full-stack event management system designed for the South African road running, walking, and cycling community. This repository contains the *Part 2 implementation*, which includes a RESTful API for data management, an MVC frontend for user interaction, and a SQL Server database.

## Features
- User registration and login with role-based access (Admin / Organizer / Participant)
- Session-based authentication using ASP.NET Core Identity
- Organizer Dashboard to view event statistics
- Admin User Roles Management page
- RESTful API endpoints for Auth, Events, and Venues
- Swagger integration for API testing
- Unit tests with xUnit and EF Core InMemory

## Technologies Used
- ASP.NET Core 8.0 (MVC + Web API)
- Entity Framework Core (Code-First)
- SQL Server
- ASP.NET Core Identity for authentication
- xUnit for unit testing
- GitHub Actions for CI/CD

## User Roles

### Admin
- View and manage user roles via the "Manage Users" page
- Full access to the system

### Organizer
- Create and manage events and venues
- View dashboard statistics (total events, categories, enrolments)
- Capture race results

### Participant
- Browse and enrol in events
- View personal performance history

#GITHUB ACTIONS WORKFLOW
<img width="1430" height="712" alt="image" src="https://github.com/user-attachments/assets/98fe2f74-940c-477e-b29c-76cf62eecdef" />

## Video Walkthrough

Watch the video walkthrough of the RaceDayy Event Management System to see its main features, user roles, dashboards, API functionality, and testing.

**Video Link:** [Watch the RaceDayy Walkthrough](https://youtu.be/MFFXlcaDqYo)

## Setup Instructions

### Prerequisites
- Visual Studio 2022
- .NET 8.0 SDK
- SQL Server (Express or Developer edition)

### Running the Project
1. Clone the repository.
2. Open RaceDayy.sln in Visual Studio.
3. Ensure the connection string in appsettings.json points to your local SQL Server.
4. Open the Package Manager Console and run:
   ```powershell
   Update-Database -Context ApplicationDbContext# RaceDayy
**Student Name:** Indiphile Diko  
**Project:** RaceDayy Event Management System  
