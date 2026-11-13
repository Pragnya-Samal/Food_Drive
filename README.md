# Food Drive — Surplus Food Redistribution & Management System

A role-based web platform designed to solve food waste problem  by connecting restaurants, event organizers, and individual donors with recipients and community organizations to redistribute surplus food efficiently.

---

## Key Features

* **Role-Based Authentication & Access Control:** Powered by **Supabase Auth**, supporting email/password registration, password recovery, and Google/Facebook OAuth sign-in across **Admin**, **Donor**, and **Recipient** roles.
* **Donor Dashboard:** Track total donations and recipient impact metrics, build multi-item food donation lists with allergen/handling notes, schedule pickup windows and addresses, and monitor delivery statuses (`Processing`, `Scheduled`, `Delivered`).
* **Recipient Dashboard:** Browse real-time available food items with stock status and per-order quantity limits, manage a selection cart, and schedule pickups[cite: 3].
* **Admin Dashboard:** Centralized management interface for monitoring food inventory, processing orders, managing users, and viewing system reports[cite: 3].
* **Community & Engagement Pages:** Dedicated views for platform overview (`About Us`), menu listings, contact inquiries, and user feedback/reviews[cite: 3].

---

## Tech Stack

* **Frontend:** HTML5, CSS3, Vanilla JavaScript (ES6+), Bootstrap 5, Font Awesome, Google Fonts (Inter & Roboto)[cite: 3]
* **Backend & Authentication:** Supabase (`@supabase/supabase-js` v2) for user authentication, metadata role management, and cloud database integration[cite: 3]

---

## Project Structure

```text
fms/
├── index.html                  # Landing page with dynamic auth state navigation
├── signup.html                 # Multi-role user registration (Admin, Donor, Customer)
├── registration.html           # Role-based login & password reset portal
├── auth.js                     # Supabase client initialization & auth helper functions
├── donor.html                  # Donor dashboard, donation scheduler & history tracker
├── recipitent-dashboard.html   # Recipient food catalog & cart claiming interface
├── admin-dashboard.html        # Admin inventory, order & user management panel
├── menu2.html                  # Food items catalog view
├── order.html                  # Order summary and checkout view
├── profile.html                # User profile and order history
├── aboutus.html                # Mission and food waste reduction overview
├── contactus.html              # Contact & support page
├── feedback.html               # User feedback and reviews page
└── *.css / *.jpg               # Component stylesheets and visual assets
