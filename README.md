# 🏡 RealEstate Pro  
**Enterprise-Grade Real Estate Marketplace built with Laravel (TALL Stack)**


RealEstate Pro is a full-stack web application designed to manage **Buy, Sell, and Rent** property workflows for modern real estate agencies.  
It combines a clean public marketplace with powerful role-based dashboards for **Admins** and **Agents**, focusing on scalability, security, and real-time user experience.


> This project is built as a production-oriented portfolio system, not a basic CRUD demo.


---


## 🚀 Key Highlights


- Role-Based Access Control (RBAC) using **Spatie Laravel-Permission**
- Real-time UI updates with **Livewire** (no page reloads)
- Separate dashboards for Admins and Agents
- Advanced property search & filtering
- Centralized inquiry and lead management
- Clean relational database design with seeders


---


## 🖼 UI Preview


Screenshots are stored in the `/screenshots` directory.


### Landing Page
![Landing Page](screenshots/landing-page.png)


### Property Details
![Property Details](screenshots/property-detail.png)


### Admin Dashboard
![Admin Dashboard](screenshots/admin-dashboard.png)


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
🔐 Demo Credentials
Role	Email	Password
Admin	admin@example.com
	password
Agent	agent@example.com
	password
📈 Future Enhancements

Map-based property search (Google Maps / OpenStreet Maps)

Payment and booking integration

Property analytics dashboard

REST API for mobile applications

Multi-language support

👨‍💻 Author

Muhammad Tayyab
BS Computer Science
Core Stack: Laravel, MERN, Full-Stack Web Development

This project reflects a focus on building scalable backend systems, clean RBAC implementation, and production-ready architecture.
