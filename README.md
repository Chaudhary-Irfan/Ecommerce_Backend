# Ecommerce Backend

This is the backend API for the Ecommerce application built with **Laravel 11** and **MySQL**. It provides all the endpoints for managing products, orders, users, and cart functionalities.

## 🚀 Features

- CRUD operations for products
- Cart and order management
- Database seeding with sample data
- RESTful API structure
- Exception handling and validation

## 🛠 Tech Stack

- **Framework:** Laravel 11
- **Database:** MySQL (via XAMPP / phpMyAdmin)
- **Language:** PHP 8.4+
- **Composer** for dependency management

## ⚙️ Setup Instructions

1. **Clone the repository**
```bash
git clone <backend-repo-url>
cd ecommerce-backend
Install dependencies

composer install


Configure environment variables

Copy .env.example to .env

cp .env.example .env


Update database credentials in .env

DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=ecommerce
DB_USERNAME=root
DB_PASSWORD=


Generate application key

php artisan key:generate


Run migrations and seed database

php artisan migrate --seed


Start the development server

php artisan serve


The backend will be available at: http://127.0.0.1:8000

🧪 Testing API Endpoints

You can use tools like Postman or Insomnia to test all API endpoints:

GET /api/products – List all products

GET /api/products/{id} – Get product details

POST /api/orders – Place an order

POST /api/cart – Add product to cart

DELETE /api/cart/{id} – Remove product from cart

(More endpoints are available in the API documentation or routes file)

⚡ Notes

Ensure MySQL service is running via XAMPP.

Run composer dump-autoload if new classes are added.

Enable required PHP extensions: pdo, pdo_mysql, openssl.