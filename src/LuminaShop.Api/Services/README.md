# Services Directory

This directory contains business logic services that implement the application's core functionality.

## Structure

- **IProductService.cs / ProductService.cs** - Product business logic
- **IOrderService.cs / OrderService.cs** - Order business logic
- **IImportService.cs / ImportService.cs** - Data import logic (Excel/CSV)
- **IExcelImportService.cs / ExcelImportService.cs** - Excel-specific import
- **ICsvImportService.cs / CsvImportService.cs** - CSV-specific import

## Best Practices

- Use interfaces for dependency injection
- Keep services focused on single responsibility
- Use async methods
- Validate inputs
