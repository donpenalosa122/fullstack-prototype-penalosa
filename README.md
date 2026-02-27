# PENALOSA Full-Stack Prototype
Developed by Donald M. Penalosa , this project is a role-based Single Page Application (SPA) built to demonstrate frontend architecture, client-side routing, and local data persistence.   

🚀 Project Overview
This prototype simulates a full-stack environment without the need for a backend server. It features:   


Email Registration: Includes a fake verification workflow.   


Simulated Authentication: Login system using JWT-like token simulation.   


Role-Based UI: Dynamic interfaces for both Admin and User roles.   


Full CRUD Functionality: Manage Employees, Departments, and Requests.   


Data Persistence: All application data is stored in localStorage; a refresh resets the state.   

📂 Project Structure
The project consists of a clean, modular file setup:   


index.html: The main entry point for the SPA structure.   


style.css: Custom styles for the navigation, forms, and tables.   


script.js: Contains the logic for routing, authentication, and data handling.   


README.md: Project documentation and progress tracking.   

🛠️ Installation & Setup

Clone the repository:    

Bash
git clone https://github.com/donpenalosa122/fullstack-prototype-penalosa.git
Navigate to the directory:

Bash
cd fullstack-prototype-penalosa
Run the app:
Simply open index.html in any modern web browser.

🔧 Git Workflow & Development
This project follows a systematic development phase:


Phase 0: Setup & Planning — Initializing files and repository.   


Phase 1: Core Structure & Navigation — Building the Home, Login, and Register pages.   


Bug Fixes: Resolved a critical TypeError where the "backdrop" would orphan in the DOM during navigation.   

Key Bug Fix Implementation
To ensure the UI doesn't freeze when navigating while a modal is open, a global cleanup routine was added to the showPage function:   

JavaScript
document.querySelectorAll('.modal-backdrop').forEach(el => el.remove());
document.body.classList.remove('modal-open');
🖥️ Features & Screenshots

Registration/Login: User sign-up with password length validation of at least 6 characters.   


Admin Dashboard: Full access to manage Employees (ID, Position, Hire Date) and Departments.   


Request System: Users can submit equipment requests with specific item names and quantities.
