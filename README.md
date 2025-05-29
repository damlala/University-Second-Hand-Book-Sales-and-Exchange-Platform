# Book-Sale-Website
This is a project that people can buy, sale, exchange or donate books.
System Requirements
Visual Studio 2022 or later (.NET 6 SDK included)
PostgreSQL (v14+)
pgAdmin4
A modern browser (e.g., Google Chrome)
.NET 6 SDK
NuGet package manager (built into Visual Studio)

1. Set Up the PostgreSQL Database
Download and install PostgreSQL and pgAdmin if not already installed.
Open pgAdmin and create a new database named: bookexchange
Open a terminal and start PostgreSQL manually if needed:
"C:\Program Files\PostgreSQL<version>\bin\pg_ctl.exe" -D "C:\PostgresData" start

Make sure your appsettings.json file contains the following connection string:
"ConnectionStrings": {
"DefaultConnection": "Host=localhost;Port=5432;Database=bookexchange;Username=postgres;Password=Admin123!"
}

2. Run the Backend (.NET 6 Web API)
Open the solution in Visual Studio 2022
Restore NuGet packages if prompted
Build the solution (Ctrl + Shift + B) to ensure dependencies are resolved
Run the project using IIS Express or Kestrel
➤ API will run at: http://localhost:5052
Swagger UI will be available at: http://localhost:5052/swagger

3. Access the Admin Panel
Open your browser and go to: http://localhost:5052/admin.html
Use default credentials to log in:
Username: admin
Password: admin123
Admin can view, delete users and books

4. Access the User Interface
Open your browser and go to: http://localhost:5052/proje.html
Register as a user and start using the platform to list, search, or add books to cart

5. Run Notes
PostgreSQL must be running before launching the backend
Make sure port 5052 is not blocked or used by other services
You may test API endpoints directly via Swagger UI if needed
