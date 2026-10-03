# Graphic Designer Portfolio Website

A complete graphic designer portfolio website built using HTML, CSS, JavaScript, PHP, and MySQL for use with XAMPP/Apache.

## Requirements

- XAMPP with Apache and MySQL enabled
- PHP 8+
- Modern browser
- MySQL database access via phpMyAdmin or MySQL CLI

## XAMPP Setup

1. Install XAMPP.
2. Start Apache and MySQL.
3. Place the project folder inside `htdocs`.
4. Open phpMyAdmin and create the database `graphic_designer_portfolio`.
5. Import the SQL file from `database/database.sql`.

## Database Setup

1. Open phpMyAdmin.
2. Create a database named `graphic_designer_portfolio`.
3. Import the file:
   - `database/database.sql`
4. Confirm tables are created:
   - `admins`
   - `categories`
   - `projects`
   - `testimonials`
   - `messages`
   - `hire_requests`
   - `settings`

## Configuration

Edit the database credentials in `php/config/database.php` if needed:

```php
$host = '127.0.0.1';
$dbName = 'graphic_designer_portfolio';
$username = 'root';
$password = '';
```

## Run the Project

1. Copy the project folder into `C:/xampp/htdocs/`.
2. Navigate to `http://localhost/graphic-designer-portfolio/`
3. For admin, go to `http://localhost/graphic-designer-portfolio/admin/`

## Admin Login

Default admin account:

- Email: `admin@designer.com`
- Password: `admin123`

## Folder Structure

- `index.html` – home page
- `portfolio.html` – portfolio gallery
- `project-details.html` – project details page
- `services.html` – services listing
- `testimonials.html` – testimonials page
- `contact.html` – contact form
- `admin/` – admin dashboard and management pages
- `css/` – site styling
- `js/` – JS behavior and AJAX logic
- `php/` – backend APIs and auth
- `database/` – SQL schema and seed data

## Adding Portfolio Projects

1. Log into the admin panel.
2. Go to Add Work.
3. Upload a project image.
4. Fill in title, category, client, date, tools, description.
5. Save the project.

## Changing Contact Information

1. Log into the admin panel.
2. Open Settings.
3. Update the designer name, email, phone, WhatsApp, location, and social media URLs.
4. Save the changes.

## Notes

- The site uses HTML, CSS, JavaScript, PHP, and MySQL in a separated architecture.
- Frontend pages use JavaScript fetch requests to PHP API files.
- The admin area requires session-based authentication.
