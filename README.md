# AMPD.LiveStockManagementV9.8
A comprehensive livestock management system built with .NET 8.0
# AMPD Live Stock Management System

A comprehensive livestock management system built with .NET 8.0, featuring modules for animal management, breeding, health tracking, commercial operations, financial management, and security.

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

### 6. Security Module
- Incident tracking and reporting
- Security event logging
- Access control management
- Security metrics

## System Requirements

- Docker Desktop
- Visual Studio 2022
- .NET 8.0 SDK

## Running the Application

### Option 1: Using Docker (Recommended)

1. Clone the repository
2. Open terminal in the project root directory
3. Run:
```bash
docker-compose up --build
```

The application will be available at:
- Web Interface: http://localhost:8080

### Option 2: Using Visual Studio 2022

1. Open `AMPD Live Stock Management.sln`
2. Set `AMPD Live Stock Management` as startup project
3. Press F5 to run

## Project Structure

```
AMPD Live Stock Management/
├── Controllers/           # Application controllers
├── Models/               # Data models and mock data
├── Views/                # MVC views for each module
├── wwwroot/             # Static files (CSS, JS, images)
└── Properties/          # Application properties
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
