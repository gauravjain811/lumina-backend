# Models Directory

This directory contains data models, entities, and DTOs.

## Structure

- **Entities/** - EF Core entity models
  - Product.cs
  - Order.cs
  - OrderItem.cs
  - Customer.cs
- **Dtos/** - Data Transfer Objects
  - CreateProductDto.cs
  - UpdateProductDto.cs
  - CreateOrderDto.cs
  - OrderResponseDto.cs

## Best Practices

- Entities map to database tables
- DTOs are used for API requests/responses
- Use data annotations for validation
