# LuminaShop - Backend API

Enterprise e-commerce API built with **.NET 9** and **ASP.NET Core**. Handles product management, orders, and data processing from Excel/CSV imports.

## Tech Stack

- **Framework**: .NET 9
- **Web Framework**: ASP.NET Core
- **Language**: C# 13
- **Database**: SQL Server (configurable)
- **Data Processing**: Excel, CSV parsing
- **API Standard**: RESTful with OpenAPI/Swagger

## Project Structure

```
lumina-backend/
├── src/
│   └── LuminaShop.Api/
│       ├── Controllers/          # API endpoint controllers
│       ├── Services/             # Business logic services
│       ├── Models/               # Data models and DTOs
│       ├── Data/                 # Entity Framework DbContext
│       ├── Repositories/         # Data access layer
│       ├── Middleware/           # Custom middleware
│       ├── Config/               # Configuration classes
│       ├── Filters/              # Action filters
│       ├── Validators/           # FluentValidation validators
│       ├── Migrations/           # EF Core migrations
│       ├── appsettings.json      # Configuration
│       ├── Program.cs            # Application entry point
│       └── LuminaShop.Api.csproj
├── tests/
│   └── LuminaShop.Api.Tests/     # Unit and integration tests
├── docs/
│   └── API.md                    # API documentation
├── README.md                     # This file
└── .gitignore                    # Git ignore patterns
```

## Features

- ✅ RESTful API endpoints
- ✅ Entity Framework Core ORM
- ✅ Excel/CSV data import
- ✅ Input validation with FluentValidation
- ✅ Dependency Injection
- ✅ Async/await patterns
- ✅ OpenAPI/Swagger documentation
- ✅ Authentication & Authorization ready
- ✅ Structured exception handling
- ✅ Logging support

## Getting Started

### Prerequisites

- .NET 9 SDK
- SQL Server (or configure another database)
- Visual Studio 2022 or VS Code

### Setup

```bash
# Clone the repository
git clone https://github.com/gauravjain811/lumina-backend.git
cd lumina-backend

# Restore dependencies
dotnet restore

# Navigate to API project
cd src/LuminaShop.Api

# Apply database migrations
dotnet ef database update

# Run the application
dotnet run
```

### Development Server

The API will be available at `https://localhost:5001`
Swagger UI: `https://localhost:5001/swagger`

### Build

```bash
# Build the project
dotnet build

# Build for release
dotnet publish -c Release
```

### Testing

```bash
# Run all tests
dotnet test

# Run specific test project
dotnet test tests/LuminaShop.Api.Tests/
```

## API Endpoints

### Products
- `GET /api/products` - Get all products
- `GET /api/products/{id}` - Get product by ID
- `POST /api/products` - Create product
- `PUT /api/products/{id}` - Update product
- `DELETE /api/products/{id}` - Delete product

### Orders
- `GET /api/orders` - Get all orders
- `GET /api/orders/{id}` - Get order by ID
- `POST /api/orders` - Create order
- `PUT /api/orders/{id}` - Update order status

### Data Import
- `POST /api/import/products` - Import products from Excel/CSV
- `GET /api/import/status` - Check import status

## Configuration

Edit `appsettings.json` to configure:
- Database connection string
- Logging levels
- API settings

## Contributing

1. Create a feature branch (`git checkout -b feature/amazing-feature`)
2. Commit changes (`git commit -m 'Add amazing feature'`)
3. Push to branch (`git push origin feature/amazing-feature`)
4. Open a Pull Request

## License

MIT License - see LICENSE file for details

## Project Links

- **Frontend UI**: https://github.com/gauravjain811/lumina-ui
- **Test Suite**: https://github.com/gauravjain811/lumina-automation
