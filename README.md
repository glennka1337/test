# Fjordingarnas Bokningssystem

A web-based booking system designed for barbers to manage appointments, customers, employees, and services efficiently. Built using ASP.NET Core with a clean architecture approach that separates concerns across Controllers, Services, Repositories, and Models.

## 🧰 Tech Stack

- **Backend**: ASP.NET Core Web API  
- **Database**: Entity Framework Core (Code First)  
- **Architecture**: Layered (API, Repositories, Services, DTOs, Models)  
- **Testing**: Unit Tests with xUnit (in `BookingSystem.Tests`)

---

## 📁 Project Structure

- **BookingSystem.API** – Main API project  
  - `Controllers/` – Handles HTTP requests for bookings, customers, employees, and services  
  - `Data/` – Contains `AppDbContext` and EF Core migrations  
  - `Models/` – Entity models and DTOs  
  - `Repositories/` – Interfaces and implementations for data access  
  - `Services/` – Core business logic  

- **BookingSystem.Tests** – Unit tests  
- **Fjordingarnas_Bokningssystem** – Likely for service registration and shared services  
- **Models** – Core entities: `Customer`, `Booking`, `Service`, `Employee`

---

## 🚀 Features

- 📆 **Book Appointments**: Schedule and manage bookings by date and time  
- 💇 **Service Management**: Create and update services (e.g., haircut, shave)  
- 👥 **Customer Profiles**: View and manage customer information  
- 👨‍🔧 **Employee Assignments**: Assign services and bookings to employees  
- 📊 **DTOs** for clean and safe data transfer  
- 🔄 **Rescheduling Support**: Update and move bookings as needed  

---

## 🛠️ Getting Started

### Prerequisites

- [.NET 8 SDK](https://dotnet.microsoft.com/download)  
- SQL Server or LocalDB  
- Visual Studio or VS Code  

### Setup

1. **Clone the repository**

```bash
git clone https://github.com/SerhanGyuler/Fjordingarnas_Bokningssystem.git
cd Fjordingarnas_Bokningssystem
```

2. **Apply EF Core migrations**

```bash
cd BookingSystem.API
dotnet ef database update
```

3. **Run the API**

```bash
dotnet run --project BookingSystem.API
```

4. **Test the endpoints**

Use Postman or the included `Bookingsystem.API.http` file to test endpoints like:
- `/api/booking`
- `/api/customer`
- `/api/employee`
- `/api/service`

---

## 🧪 Running Tests

```bash
dotnet test BookingSystem.Tests
```

---

## 📸 Screenshots

*Add screenshots of the API in use or database structure if available.*

---

## 📌 TODO / Future Improvements

- Add Swagger UI for easy API documentation  
- Add authentication (JWT or Identity)  
- Build a front-end interface (e.g., Blazor, React)  
- SMS or Email booking confirmation  

---

## 📄 License

MIT License

---

## 👤 Author

**Serhan Gyuler**  
[GitHub Profile](https://github.com/SerhanGyuler)
