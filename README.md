# TodoApi Minimal API

A simple Minimal API built with ASP.NET Core 8.  
This project implements a basic CRUD API for to-do items using an in-memory database.  
It’s perfect for learning how Minimal APIs work in .NET.

Based on the official Microsoft tutorial:  
https://learn.microsoft.com/en-us/aspnet/core/tutorials/min-web-api?view=aspnetcore-8.0&tabs=visual-studio-code

---

## Endpoints

GET    /todoitems           - Get all items  
GET    /todoitems/complete  - Get completed items  
GET    /todoitems/{id}      - Get item by ID  
POST   /todoitems           - Create new item  
PUT    /todoitems/{id}      - Update item by ID  
DELETE /todoitems/{id}      - Delete item by ID  

---

## Getting Started

1. Clone the repository:
   git clone <your-repo-url>
   cd <project-folder>

2. Restore dependencies:
   dotnet restore

3. (Optional) Add required packages:
   dotnet add package Microsoft.EntityFrameworkCore.InMemory  
   dotnet add package Microsoft.AspNetCore.Diagnostics.EntityFrameworkCore --version 8.0.0  
   dotnet add package NSwag.AspNetCore  

4. Build and run:
   dotnet build  
   dotnet run

5. Open in your browser or Postman:
   https://localhost:5001/swagger  

---

## Notes

- Data is stored in-memory (resets after restart).  
- Not intended for production use.  
- You can easily extend it with a real database or additional features.
