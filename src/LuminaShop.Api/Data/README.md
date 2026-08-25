# Data Directory

This directory contains Entity Framework Core DbContext and related database configurations.

## Structure

- **LuminaDbContext.cs** - Main DbContext class
- **Configurations/** - Entity configurations
  - ProductConfiguration.cs
  - OrderConfiguration.cs
  - CustomerConfiguration.cs

## Migrations

Database migrations are managed using EF Core CLI:

```bash
# Create a new migration
dotnet ef migrations add MigrationName

# Apply migrations
dotnet ef database update

# Revert last migration
dotnet ef migrations remove
```
