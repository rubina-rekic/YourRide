# 🚗 YourRide – ASP.NET Web Application

YourRide is a full-stack ride-sharing web application built using ASP.NET Core. The platform connects passengers with drivers, supporting real-time notifications, role-based access control, and a complete ride management workflow. Developed as a collaborative university project to demonstrate advanced software engineering principles and clean architecture.

---

## ✨ Features

- 👤 **User Management** — Secure registration, login and access control powered by ASP.NET Core Identity
- 🚕 **Ride Management** — End-to-end workflow for passengers to request rides and drivers to respond
- 🔔 **Real-time Notifications** — SignalR keeps passengers and drivers in sync without refreshing the page
- 🔐 **Role-based Access Control** — Four distinct roles, each with their own dashboard and permissions:
  - `Putnik` — Passenger: request and track rides
  - `Vozač` — Driver: accept and manage ride requests
  - `Administrator` — Full system management
  - `TehnickaPodrska` — Technical support access
- 🏗 **MVC Architecture** — Controllers handle logic, Views handle display, Models handle data — keeping the codebase clean and maintainable

---

## 🏗 Architecture & Design

This project includes comprehensive documentation covering the full system design:

- **Design Patterns** — SOLID principles applied throughout, with examples of Decorator, Composite and other patterns
- **UML Diagrams** — Use Case, Class, Sequence and Activity diagrams
- **Database Design** — Full Entity Relationship Diagram (ERD)

---

## 🛠 Technologies

| Layer | Technology |
|-------|-----------|
| Backend | C# / ASP.NET Core |
| ORM | Entity Framework Core |
| Frontend | ASP.NET MVC, Razor Pages, HTML5, CSS3, JavaScript |
| Real-time | SignalR |
| Auth | ASP.NET Core Identity |
| Database | SQL Server / LocalDB |

---

## 📁 Documentation

All diagrams and architectural specifications are in the `Dokumentacija` folder, covering the complete software development lifecycle from requirements analysis through to design patterns implementation.

---

## 🚀 How to Run

### Prerequisites
- Visual Studio 2022+
- .NET SDK
- SQL Server or LocalDB (included with Visual Studio)

### Steps

**1. Clone the repository**
```bash
git clone https://github.com/rubina-rekic/YourRide.git
cd YourRide
```

**2. Configure the database connection**

Open `appsettings.json` and set your connection string:
```json
"ConnectionStrings": {
  "DefaultConnection": "Server=(localdb)\\mssqllocaldb;Database=YourRide;Trusted_Connection=True;MultipleActiveResultSets=true"
}
```

**3. Apply database migrations**

In Visual Studio, open **Tools → NuGet Package Manager → Package Manager Console** and run:
```powershell
Update-Database
```

**4. Run the application**

Press **F5** or click the Run button in Visual Studio.

---

## 👥 Team

- Rubina Rekić
- Irma Topčagić
- Irma Lemeš

*University project — Faculty of Electrical Engineering, Sarajevo*
*Object-Oriented Analysis and Design — Academic Year 2024/25*
