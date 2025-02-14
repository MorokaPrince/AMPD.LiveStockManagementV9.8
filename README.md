# AMPD LiveStock Management System v9.8

## Project Overview
A comprehensive livestock management system built with ASP.NET Core 8.0, designed to help farmers and ranchers manage their livestock operations efficiently.

## Features
- Animal tracking and management
- Health records management
- Breeding records tracking
- Financial transaction monitoring
- Dashboard with key metrics

## Technical Stack
- ASP.NET Core 8.0
- Entity Framework Core
- SQL Server
- Docker support
- Bootstrap 5

## Project Structure
```bash
AMPD.LiveStock/
├── Controllers/               # MVC Controllers
├── Models/                    # Domain Models
├── Data/                      # Database Context and Configurations
├── Views/                    # MVC Views
├── wwwroot/                 # Static files
├── Services/                # Business logic layer
└── Properties/              # Project properties
```

## Getting Started
1. Clone the repository
2. Install .NET 8.0 SDK
3. Run `dotnet restore`
4. Run `dotnet run`

## Docker Support
```bash
docker-compose up --build
```

## License
MIT License