# Talabat.Api – E-Commerce Web API (.NET 8)
Talabat.Api is a backend RESTful API built using ASP.NET Core 8, inspired by the food delivery and e-commerce domain. This project provides robust endpoints for handling user registration, authentication, product browsing, basket (cart) management, and order processing.

🚀 Technologies Used
⚙️ .NET 8 (ASP.NET Core Web API)

🧩 Entity Framework Core (for data access and database context)

🔐 JWT Authentication (for secure user sessions)

📦 Swagger / OpenAPI (for interactive API documentation)

💾 SQL Server (or InMemoryDb for development)

📑 API Modules & Endpoints
🔐 Auth
POST /api/Auth/Register – Register a new user

GET /api/Auth/GetCurrentUser – Retrieve logged-in user info

GET /api/Auth/Address – Get saved address

PUT /api/Auth/Address – Update user address

GET /api/Auth/EmailExists – Check if email is already registered

🛒 Basket (Shopping Cart)
GET /api/Basket – Get the current user's basket

POST /api/Basket – Create or update the basket

DELETE /api/Basket – Remove the basket

📦 Orders
POST /api/Order – Place a new order

GET /api/Order – Get list of user's orders

GET /api/Order/{id} – Get specific order details

GET /api/Order/GetDeliveryMethod – Get available delivery methods

🛍️ Products
GET /api/Product – Get all products with filters

GET /api/Product/{id} – Get product by ID

GET /api/Product/GetBrands – List of brands

GET /api/Product/GetTypes – List of product types

🧱 Data Models (Schemas)
Includes DTOs and models like:

UserDto, RegisterDto

ProductDTO, ProductBrand, ProductType

BasketItemDto, CustomerBasketDto

OrderDto, OrderItemDto, DeliveryMethod

Error handling model: ApiErrorResponse

📸 Swagger UI
All API endpoints are documented with Swagger UI, making testing and development easy through an interactive interface.
Access it at: https://localhost:7285/swagger/index.html
![WhatsApp Image 2025-07-16 at 4 31 25 PM](https://github.com/user-attachments/assets/6d159448-5057-419f-a8e1-abe62873d7b2)
![WhatsApp Image 2025-07-16 at 4 31 52 PM](https://github.com/user-attachments/assets/7369f07c-9237-478b-8566-629a8c99a9a5)
![WhatsApp Image 2025-07-16 at 4 32 22 PM](https://github.com/user-attachments/assets/251fcb7a-5d36-4b7c-a548-bcd7068cf1a7)
![WhatsApp Image 2025-07-16 at 4 32 52 PM](https://github.com/user-attachments/assets/6efa5236-d64f-4ebd-a5bf-a104328b71a6)


✅ Features
Fully modular and layered architecture (Controller → Service → Repository)

JWT-based Authentication & Authorization

Swagger for testing and development

Clean separation of DTOs and domain models

Includes basic validation and error responses

🏗️ Future Improvements
Admin panel (with product and order management)

Payment gateway integration

Email notifications

Role-based access control

