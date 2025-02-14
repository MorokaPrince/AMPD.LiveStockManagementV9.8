# AMPD LiveStock Management System v9.8

## Project Overview
A comprehensive livestock management system built with ASP.NET Core 8.0, designed to help farmers and ranchers manage their livestock operations efficiently.

## System Features

### 1. Animal Management Module
- Complete animal inventory tracking
- Individual animal profiles and history
- Animal categorization and grouping
- Movement and location tracking
- Custom attributes and tags

### 2. Breeding Management
- Breeding records and history
- Genealogy tracking
- Breeding schedule management
- Offspring tracking
- Performance metrics

### 3. Health Management
- Vaccination schedules and records
- Health incident tracking
- Treatment records
- Medical history
- Health statistics and reporting
- Upcoming health events calendar

### 4. Commercial Operations
- Product inventory tracking
- Sales management
- Product categorization
- Performance metrics
- Stock monitoring

### 5. Financial Management
- Custom fiscal year management (April-March)
- Expense tracking
- Accounts receivable
- Financial dashboard with KPIs
- Excel report generation
- Financial projections

## Technical Stack
- ASP.NET Core 8.0
- Entity Framework Core
- SQL Server
- Docker support
- Bootstrap 5

## Getting Started
1. Clone the repository
2. Install .NET 8.0 SDK
3. Run `dotnet restore`
4. Run `dotnet run`

## Docker Support
```bash
docker-compose up --build
```

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

## Development Mode

The application currently uses mock data for development and demonstration:
- Pre-configured sample data for all modules
- In-memory data storage
- No database setup required
- Ideal for UI/UX development and testing

## Docker Configuration

Single container setup for the web application:
- .NET 8.0 web application
- Exposed on port 8080
- Uses in-memory mock data
- Hot reload enabled for development

## Troubleshooting

### Docker Issues
1. Clean up existing containers:
```bash
docker-compose down
```

2. Rebuild container:
```bash
docker-compose up --build
```

### Application Issues
1. Check application logs:
```bash
docker-compose logs
```

2. Verify service is running:
```bash
docker-compose ps
```

## Development Guidelines

1. **Mock Data**
   - Mock data is located in Models directory
   - Update mock data to test different scenarios
   - Keep mock data realistic for testing

2. **Docker Development**
   - Use docker-compose.override.yml for local customizations
   - Keep Dockerfile optimized for development
   - Test builds before committing

## Future Enhancements

1. **Database Integration**
   - PostgreSQL integration planned
   - Data persistence implementation
   - Migration from mock to real data

2. **Additional Features**
   - Enhanced reporting
   - Advanced analytics
   - Mobile responsiveness
   - API endpoints

## Support and Maintenance

For technical support or questions:
1. Check the troubleshooting guide
2. Review application logs
3. Contact the development team

## Security Considerations

1. **Application Security**
   - Built-in authentication and authorization
   - Role-based access control
   - Regular security updates
