🏡 RealEstate Pro
Enterprise-Grade Real Estate Marketplace built with Laravel (TALL Stack)
RealEstate Pro is a full-stack web application designed to manage Buy, Sell, and Rent property workflows for modern real estate agencies.
It combines a clean public marketplace with powerful role-based dashboards for Admins and Agents, focusing on scalability, security, and real-time user experience.
This project was built as a production-oriented portfolio system, not a demo CRUD app.
________________________________________
🚀 Key Highlights
•	Role-based access control using Spatie Permissions
•	Real-time UI with Livewire (no page reloads)
•	Separate Admin & Agent dashboards
•	Advanced property search & filtering
•	Centralized inquiry / lead management
•	Clean database design with seeders
________________________________________
🖼 UI Preview
Screenshots are stored in the /screenshots directory.
Landing Page

Property Details

Admin Dashboard

Admin Dashboard Property Management

________________________________________
🧠 System Architecture
The application follows a modular Laravel architecture, separating public-facing functionality from administrative control.
Tech Stack
Layer	Technology
Backend	Laravel 11
Frontend	Livewire
UI	Tailwind CSS + Bootstrap
Client Interactions	Alpine.js
Authentication & RBAC	Spatie Laravel-Permission
Database	MySQL
Storage	Laravel Public Storage
________________________________________
👥 User Roles & Access Control
The system enforces strict Role-Based Access Control (RBAC).
Role	Capabilities
Admin	Full system access: manage users, agents, listings, permissions, and inquiries
Agent	Create, update, delete only their own property listings
Customer / Guest	Browse listings and submit property inquiries
Permissions are managed centrally using Spatie’s permission gates and policies.
________________________________________
🧩 Functional Modules
1. Public Marketplace
Accessible to all visitors.
•	Property search by:
o	Property Type (House, Plot, Flat, Commercial)
o	City / Location
o	Price Range
o	Bedrooms & Bathrooms
•	Featured & latest listings
•	SEO-friendly property detail pages
•	Integrated inquiry form (Email, Phone, WhatsApp)
________________________________________
2. Admin Dashboard
A centralized control panel for platform management.
•	Global property CRUD operations
•	Agent creation & verification
•	License & agency management
•	Inquiry / lead tracking
•	Platform-level statistics (users, listings, activity)
________________________________________
3. Agent Dashboard
Designed for real estate professionals.
•	Manage personal property listings
•	Draft & publish workflow
•	Restricted access to own data only
•	Clean, focused UI for productivity
________________________________________
🗄 Database Design (Overview)
The system uses a relational schema optimized for integrity and scalability.
Table	Purpose
users	Authentication & base user data
roles / permissions	RBAC management
properties	Core property listings
agents	Professional agent profiles
inquiries	Customer messages & leads
Seeders automatically initialize roles, permissions, and demo data.
________________________________________
⚙️ Installation & Setup
Prerequisites
•	PHP 8.2+
•	Composer
•	Node.js & NPM
•	MySQL
Steps
git clone https://github.com/your-username/realestate-pro.git
cd realestate-pro
composer install
npm install && npm run build
cp .env.example .env
php artisan key:generate
php artisan migrate --seed
php artisan storage:link
php artisan serve
________________________________________
🔐 Demo Credentials
Role	Email	Password
Admin	admin@example.com	password
Agent	agent@example.com	password
________________________________________
📈 Future Enhancements
•	Map-based property search (Google / OpenStreet Maps)
•	Payment & booking integration
•	Property analytics dashboard
•	REST API for mobile applications
•	Multi-language support
________________________________________
👨‍💻 Author
Muhammad Tayyab
BS Computer Science
Core Stack: Laravel, MERN, Full-Stack Web Development
This project reflects my focus on building structured, scalable backend systems with clean role-based access control.
________________________________________
📄 License
This project is open-source under the MIT License.

