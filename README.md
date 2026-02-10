#  RealEstate Pro  

**Enterprise-Grade Real Estate Marketplace built with Laravel (TALL Stack)**

RealEstate Pro is a full-stack web application designed to manage **Buy, Sell, and Rent** property workflows for modern real estate agencies.  
It combines a clean public marketplace with powerful role-based dashboards for **Admins** and **Agents**, focusing on scalability, security, and real-time user experience.

> This project is built as a production-oriented portfolio system, not a basic CRUD demo.

---


##  Key Highlights

- Role-Based Access Control (RBAC) using **Spatie Laravel-Permission**
- Real-time UI updates with **Livewire** (no page reloads)
- Separate dashboards for Admins and Agents
- Advanced property search & filtering
- Centralized inquiry and lead management
- Clean relational database design with seeders

---


##  UI Preview

### Admin Dashboard
![landing page](https://github.com/tayyab007-dot/property-management-system/blob/main/Admin%20dashboard.png?raw=true)

### Property Details
![property detail](https://github.com/tayyab007-dot/property-management-system/blob/main/property%20details.png?raw=true)

### Landing Page
![landing page](https://github.com/tayyab007-dot/property-management-system/blob/main/landing%20page.png?raw=true)

### Admin Dashboard Property Management
![dashboard management](https://github.com/tayyab007-dot/property-management-system/blob/main/properties%20management.png?raw=true)

---


## 🧠 System Architecture

The application follows a **modular Laravel architecture**, separating public-facing functionality from administrative control.

### 🛠 Tech Stack

| Layer | Technology |
|-----|-----------|
| Backend | Laravel 11 |
| Frontend | Livewire |
| UI Styling | Tailwind CSS + Bootstrap |
| Client Interactivity | Alpine.js |
| Authentication & RBAC | Spatie Laravel-Permission |
| Database | MySQL |
| File Storage | Laravel Public Storage |

---


## 👥 User Roles & Access Control

The system enforces strict **Role-Based Access Control (RBAC)**.

| Role | Capabilities |
|----|-------------|
| **Admin** | Full system access: manage users, agents, properties, permissions, and inquiries |
| **Agent** | Create, update, and delete **only their own** property listings |
| **Customer / Guest** | Browse properties and submit inquiries |

Permissions are handled using policies, middleware, and Spatie permission gates.

---


## 🧩 Functional Modules

### 1. Public Marketplace

Accessible to all visitors.

- Property search by:
  - Property Type (House, Plot, Flat, Commercial)
  - City / Location
  - Price Range
  - Bedrooms & Bathrooms
- Featured and latest listings
- SEO-friendly property detail pages
- Inquiry form with Email, Phone, and WhatsApp support

---


### 2. Admin Dashboard

Centralized control panel for platform management.

- Global property CRUD operations
- Agent creation and verification
- License and agency management
- Inquiry and lead tracking
- Platform-level statistics (users, listings, activity)

---


### 3. Agent Dashboard

Designed for real estate professionals.

- Manage personal property listings
- Draft and publish workflow
- Restricted access to own data only
- Clean and focused UI for productivity

---


## 🗄 Database Design (Overview)

The system uses a relational schema optimized for integrity and scalability.

| Table | Purpose |
|------|--------|
| `users` | Authentication and base user data |
| `roles` / `permissions` | Role-Based Access Control |
| `properties` | Core property listings |
| `agents` | Professional agent profiles |
| `inquiries` | Customer messages and leads |

Seeders automatically initialize roles, permissions, and demo data.

---


## ⚙️ Installation & Setup

### Prerequisites

- PHP 8.2+
- Composer
- Node.js & NPM
- MySQL

### Installation Steps

```bash
git clone https://github.com/your-username/realestate-pro.git
cd realestate-pro

composer install
npm install && npm run build

cp .env.example .env
php artisan key:generate

php artisan migrate --seed
php artisan storage:link

php artisan serve

```


## 🔐 Demo Credentials

Role	Email	Password
Admin	admin@example.com
	password
Agent	agent@example.com
	password

    
## 📈 Future Enhancements

- Map-based property search (Google Maps / OpenStreet Maps)
- Payment and booking integration
- Property analytics dashboard
- REST API for mobile applications
- Multi-language support

---

## 👨‍💻 Author

**Muhammad Tayyab**  
BS Computer Science  

**Core Stack:** Laravel, MERN, Full-Stack Web Development  

This project reflects a strong focus on building **scalable backend systems**, implementing **clean Role-Based Access Control (RBAC)**, and following **production-ready architecture principles**.
BS Computer Science
Core Stack: Laravel, MERN, Full-Stack Web Development

This project reflects a focus on building scalable backend systems, clean RBAC implementation, and production-ready architecture.
