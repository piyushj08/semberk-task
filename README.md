# semberk-task
Semberk Assignment

# URL Shortener - Laravel Assignment

A role-based URL Shortener service built with **Laravel 11** and **MySQL** as part of the Backend Developer Assignment for Sembark Tech.  
This project demonstrates authentication, authorization, company-level access rules, and secure URL redirection.

---

## 🚀 Features
- **Role Management**: SuperAdmin, Admin, Member, Sales, Manager
- **Authentication**: User login/logout with Laravel Jetstream/Sanctum
- **Invitation Rules**:
  - SuperAdmin cannot invite Admins in a new company
  - Admin cannot invite another Admin or Member in their company
- **URL Shortening Rules**:
  - Admin, Member, and SuperAdmin cannot create short URLs
  - Admin can view all URLs **not created in their own company**
  - Member can view all URLs **not created by themselves**
  - Short URLs are private (not publicly resolvable) and redirect securely
- **Database Seeder**: Creates a default SuperAdmin using raw SQL
- **Testing**: Includes unit tests for role and URL access restrictions

---

## 🛠️ Tech Stack
- **Framework**: Laravel 11
- **Language**: PHP 8+
- **Database**: MySQL
- **Auth**: Laravel Sanctum / Jetstream
- **Testing**: PHPUnit

---

## ⚙️ Installation & Setup

### 1. Clone the repository

git clone https://github.com//laravel-url-shortener.git
cd laravel-url-shortener](https://github.com/piyushj08/semberk-task/edit/main/README.md#semberk-task)

2. install dependencies

composer install
npm install && npm run dev

3. Configure environment

Copy .env.example to .env and update:

APP_NAME="URL Shortener"
APP_URL=http://localhost:8000

DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=shortener_db
DB_USERNAME=root
DB_PASSWORD=yourpassword

4. Run migrations & seeders

php artisan migrate
php artisan db:seed

5. Run the server

php artisan serve

Visit http://localhost:8000

6. Running Tests

php artisan test

Covers:

Role-based restrictions

URL access rules

Private redirection checks

### Notes

The UI is kept simple (barebones HTML) as per assignment instructions.

Used Laravel Jetstream/Sanctum for authentication scaffolding.

Default SuperAdmin credentials are configured in the DatabaseSeeder.

### AI Tools Disclosure

ChatGPT: Helped draft Eloquent relationships and project documentation.

Cursor IDE: Used for quick Laravel syntax lookup.


Login Details
 ID : superadmin@gmail.com
 password : Test@123

 



