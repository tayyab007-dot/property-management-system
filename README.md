# 🏡 RealEstate Pro

**Enterprise-Grade Real Estate Marketplace built with Laravel (TALL Stack)**

RealEstate Pro is a full-stack property management application engineered to handle **Buy, Sell, and Rent** workflows for modern real estate agencies. It integrates a public marketplace with role-based administrative dashboards for **Admins** and **Agents**, placing emphasis on security, scalability, and real-time interactive user experience.

> Designed and built as a production-oriented portfolio showcase rather than a basic CRUD application.

---

## 🌟 Key Highlights

- **Role-Based Access Control (RBAC):** Granular authorization powered by `spatie/laravel-permission`.
- **Reactive Interfaces:** Real-time state management and dynamic UI updates via **Laravel Livewire** and **Alpine.js** without page reloads.
- **Multi-Tenant Dashboards:** Isolated management portals for System Administrators and Real Estate Agents.
- **Advanced Filtering & Search:** Multi-parameter property queries (Price, Location, Category, Amenities).
- **Lead Capture System:** Direct customer inquiry funnel supporting Email and WhatsApp routing.
- **Database Architecture:** Relational schema with foreign keys, indexes, and full database seeders for instant local deployment.

---

## 🖥️ UI Preview

| Public Landing Page | Property Details View |
| :---: | :---: |
| ![Landing Page](landing%20page.png) | ![Property Details](property%20details.png) |

| Admin Control Center | Property Listing Management |
| :---: | :---: |
| ![Admin Dashboard](Admin%20dashboard.png) | ![Property Management](properties%20management.png) |

---

## 🛠️ Tech Stack & System Architecture

             +-----------------------------------+
             |           Client Layer            |
             |  Tailwind CSS | Alpine.js | Blade |
             +-----------------+-----------------+
                               |
                               v
             +-----------------------------------+
             |         Application Layer         |
             |      Laravel 11  |  Livewire      |
             +-----------------+-----------------+
                               |
                               v
             +-----------------------------------+
             |          Data & Storage           |
             |  MySQL  |  Laravel Public Storage |
             +-----------------------------------+

| Layer | Technology / Package | Function |
| :--- | :--- | :--- |
| **Backend Framework** | Laravel 11 | Core business logic, routing, and ORM |
| **Frontend Reactive** | Livewire v3 | Dynamic component state updates |
| **Client Interactivity**| Alpine.js | Lightweight DOM interactions |
| **UI Styling** | Tailwind CSS + Bootstrap | Responsive dashboard layout and components |
| **Access Control** | Spatie Laravel-Permission | Middleware, gate authorization, and role management |
| **Database** | MySQL | Relational data persistence |

---

## 👥 User Roles & Access Matrix

The system enforces authorization policies using Spatie gates and Laravel middleware.

| Feature / Action | Guest / Visitor | Agent | Admin |
| :--- | :---: | :---: | :---: |
| Browse & Search Listings | ✅ | ✅ | ✅ |
| Submit Inquiries / Leads | ✅ | ✅ | ✅ |
| Manage Personal Listings | ❌ | ✅ | ✅ |
| View Agent Dashboard | ❌ | ✅ | ✅ |
| Global User & Role Management | ❌ | ❌ | ✅ |
| Platform Analytics & Audit | ❌ | ❌ | ✅ |

---

## 🧩 Core Modules

### 1. Public Marketplace
* Dynamic multi-criteria filtering by property type, city, price range, and bedroom/bathroom count.
* Detailed listing views complete with image galleries, agent contact info, and amenity specs.
* Lead capture forms integrated with phone and email validation.

### 2. Admin Portal
* System-wide platform control over users, agents, and property approvals.
* Management of agency verification and licensing state.
* Global inquiry tracking system with status tags.

### 3. Agent Operations Portal
* Dedicated workspace for agents to create, update, and manage property portfolios.
* Strict query scoping ensuring agents access and edit **only** their assigned listings.

---

## 🚀 Installation & Local Setup

### Prerequisites
* PHP 8.2 or higher
* Composer
* Node.js (v18+) & NPM
* MySQL Database

### Setup Instructions

1. **Clone the Repository**
   ```bash
   git clone [https://github.com/tayyab007-dot/property-management-system.git](https://github.com/tayyab007-dot/property-management-system.git)
   cd property-management-system
Install PHP & Node DependenciesBashcomposer install
npm install
Configure Environment VariablesBashcp .env.example .env
php artisan key:generate
Update the .env file with your local database credentials:Code snippetDB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=realestate_db
DB_USERNAME=root
DB_PASSWORD=
Run Migrations & SeedersBashphp artisan migrate --seed
php artisan storage:link
Build Assets & Start ServerBashnpm run build
php artisan serve
Access the application at http://localhost:8000.🔐 Demo CredentialsRoleEmailPasswordAdminadmin@example.compasswordAgentagent@example.compassword🔮 Future Enhancements[ ] Map-based spatial property search using Leaflet.js or Google Maps API.[ ] Direct messaging module between buyers and listing agents.[ ] Financial calculator for mortgage and payment estimation.[ ] REST API endpoints for companion mobile applications.👨‍💻 AuthorMuhammad TayyabFull-Stack Web DeveloperGitHub: @tayyab007-dotSpecialization: Web Application Architecture, Laravel, Livewire, and Security Research.









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
