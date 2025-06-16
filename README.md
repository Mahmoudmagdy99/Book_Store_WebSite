# 📘 Book Store – ASP.NET Core MVC Web Application

A full-stack ASP.NET Core MVC web application for managing an online bookstore. This project demonstrates best practices in ASP.NET development, including layered architecture, Entity Framework Core, repository and unit of Work patterns, and Identity-based authentication and authorization.

## 🚀 Features

- ✅ User Registration and Login with ASP.NET Identity
- 🔒 Role-Based Access Control (Admin, User)
- 📚 CRUD operations for:
  - Books
  - Categories
  - Cover Types
- 🛠 Admin Dashboard for managing all data
- 🧩 Repository and Unit of Work Pattern
- 🎨 Responsive UI built with Bootstrap and Razor Views
- 🗃 Code-First Migrations using Entity Framework Core
- 💡 Clean Architecture with Dependency Injection

## 🏗️ Project Structure

```plaintext
Book_Store/
├── Bulky.DataAccess         # Data access layer (EF Core, Repositories, UoW)
├── Bulky.Models             # Data models
├── Bulky.Utility            # Static constants, helpers, and roles
├── BulkyBook.DataAccess     # Database context and seeding
├── BulkyBookWeb             # Main ASP.NET Core MVC web app
│   ├── Controllers
│   ├── Views
│   └── wwwroot              # Static files (CSS, JS, etc.)
```


## 🛠️ Technologies Used

- ASP.NET Core MVC (.NET 8)
- Entity Framework Core
- SQL Server LocalDB
- ASP.NET Identity
- Bootstrap 5
- Razor Views
- Dependency Injection
- LINQ
- Visual Studio 2022

## 🧪 Getting Started

### Prerequisites

- [.NET 8 SDK](https://dotnet.microsoft.com/download)
- [SQL Server LocalDB](https://learn.microsoft.com/en-us/sql/database-engine/configure-windows/sql-server-express-localdb)
- [Visual Studio 2022](https://visualstudio.microsoft.com/)

### Run Locally

1. Clone the repository:
   ```bash
   git clone https://github.com/Mahmoudmagdy99/Book_Store_WebSite.git
   
2- Open the solution in Visual Studio.

3-Update the appsettings.json connection string to match your SQL Server setup:
"ConnectionStrings": {
  "DefaultConnection": "Server=(LocalDb)\\MSSQLLocalDB;Database=BulkyNew;Trusted_Connection=True;TrustServerCertificate=True"
}

4-Apply migrations (Package Manager Console):
Update-Database

5-Run the project (F5 or Ctrl+F5).
