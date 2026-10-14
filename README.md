# Student Learning API

A RESTful Web API built with **C#, ASP.NET Core, Entity Framework Core, and SQL Server** to practice backend development and database operations.

## About the Project

Student Learning API is a hands-on learning project focused on building RESTful APIs using ASP.NET Core. It demonstrates how a backend application handles HTTP requests, interacts with a SQL Server database, and returns JSON responses.

## Technologies Used

- C#
- ASP.NET Core Web API
- Entity Framework Core
- Microsoft SQL Server / LocalDB
- Swagger UI
- Visual Studio

## Features

- Retrieve all student records
- Retrieve a student by ID
- Create new student records
- Update existing student records
- Delete student records
- Database integration using Entity Framework Core
- Database migrations
- API testing using Swagger UI

## Project Structure

```text
StudentLearningAPI/
├── Controllers/
├── Data/
├── Migrations/
├── Models/
├── Properties/
├── Program.cs
├── StudentLearningAPI.csproj
├── StudentLearningAPI.slnx
├── StudentLearningAPI.http
├── appsettings.json
└── README.md
```

## API Endpoints

| HTTP Method | Endpoint | Description |
|---|---|---|
| GET | `/api/Student` | Retrieve all students |
| GET | `/api/Student/{id}` | Retrieve a student by ID |
| POST | `/api/Student` | Create a student |
| PUT | `/api/Student/{id}` | Update a student |
| DELETE | `/api/Student/{id}` | Delete a student |

## Example Request

Create a student using a POST request:

```json
{
  "name": "Aman",
  "age": 21,
  "course": "C#"
}
```

## Getting Started

### Prerequisites

- .NET SDK compatible with the project
- Visual Studio
- SQL Server or SQL Server LocalDB

### Setup

1. Open `StudentLearningAPI.slnx` in Visual Studio.
2. Configure the database connection in `appsettings.json`.
3. Open the Package Manager Console.
4. Apply the existing database migrations:

   ```powershell
   Update-Database
   ```

5. Run the application.
6. Open Swagger UI using the URL displayed in the application output.

## Learning Objectives

- Understanding RESTful API architecture
- Working with HTTP methods and status codes
- Building controllers and API endpoints
- Using dependency injection
- Integrating Entity Framework Core
- Connecting to SQL Server
- Managing database migrations
- Testing APIs with Swagger UI
