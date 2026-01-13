# Laravel Online Electro Component Shop Web App

A modern e-commerce platform built with Laravel for buying and selling electronic components and skincare products. This web application provides a seamless shopping experience with user authentication, product management, shopping cart functionality, order processing, and an admin panel for managing the store.

## Features

- **User Authentication**: Secure user registration, login, and profile management using Laravel Breeze.
- **Product Management**: Browse, search, and view detailed product information including descriptions, ingredients, and usage instructions.
- **Shopping Cart**: Add products to cart, update quantities, apply coupons, and manage shipping methods.
- **Order Processing**: Place orders, view order history, and track order confirmations.
- **Admin Panel**: Comprehensive admin dashboard for managing users, orders, discounts, and store settings.
- **Blog System**: Create and view blog posts related to products and skincare tips.
- **Shoutout Feature**: Allow users to submit shoutouts or testimonials.
- **Product Comparison**: Compare multiple products side by side.
- **Responsive Design**: Mobile-friendly interface built with Tailwind CSS and Alpine.js.
- **Search Functionality**: Search for products across the catalog.

## Tech Stack

- **Backend**: Laravel 11, PHP 8.2+
- **Frontend**: Tailwind CSS, Alpine.js
- **Build Tool**: Vite
- **Database**: MySQL
- **Authentication**: Laravel Breeze
- **Testing**: Pest PHP

## Prerequisites

Before you begin, ensure you have the following installed on your system:

- PHP 8.2 or higher
- Composer (PHP dependency manager)
- Node.js and npm (for frontend assets)
- MySQL or another supported database
- Git

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/laravel-online-electro-component-shop.git
   cd laravel-online-electro-component-shop
   ```

2. **Install PHP dependencies**:
   ```bash
   composer install
   ```

3. **Install Node.js dependencies**:
   ```bash
   npm install
   ```

4. **Environment Configuration**:
   - Copy the `.env.example` file to `.env`:
     ```bash
     cp .env.example .env
     ```
   - Generate an application key:
     ```bash
     php artisan key:generate
     ```
   - Configure your database settings in the `.env` file:
     ```
     DB_CONNECTION=mysql
     DB_HOST=127.0.0.1
     DB_PORT=3306
     DB_DATABASE=your_database_name
     DB_USERNAME=your_username
     DB_PASSWORD=your_password
     ```

5. **Database Setup**:
   - Create a new MySQL database.
   - Run the migrations:
     ```bash
     php artisan migrate
     ```
   - (Optional) Seed the database with sample data:
     ```bash
     php artisan db:seed
     ```
   - Alternatively, you can import the provided `bdshop.sql` file for initial data.

6. **Build Assets**:
   ```bash
   npm run build
   ```

## Running the Application

1. **Start the Laravel development server**:
   ```bash
   php artisan serve
   ```
   The application will be available at `http://localhost:8000`.

2. **Compile and watch frontend assets** (in a separate terminal):
   ```bash
   npm run dev
   ```

3. **For production**, use the build command:
   ```bash
   npm run build
   ```

## Usage

### For Customers:
- **Browse Products**: Visit the homepage and explore the product catalog.
- **Search**: Use the search functionality to find specific products.
- **View Product Details**: Click on a product to see detailed information, ingredients, and usage instructions.
- **Add to Cart**: Add products to your shopping cart and proceed to checkout.
- **Apply Coupons**: Enter coupon codes during checkout to apply discounts.
- **Place Orders**: Complete your purchase and view order confirmations.
- **Manage Profile**: Update your profile information and view order history.
- **Compare Products**: Add products to comparison and view side-by-side details.

### For Admins:
- **Access Admin Panel**: Navigate to `/admin/login` and log in with admin credentials.
- **Manage Users**: View, edit, and delete user accounts.
- **Handle Orders**: View all orders, update shipping status, and manage order details.
- **Manage Discounts**: Create and manage discount coupons.
- **Dashboard**: Access the admin dashboard for an overview of store statistics.

## Admin Access

To access the admin panel:
1. Go to `/admin/login`
2. Use admin credentials (you may need to create an admin user via database or seeder)
3. Once logged in, access the dashboard at `/admin/dashboard`

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## Security

If you discover any security vulnerabilities, please report them responsibly by emailing the development team.
