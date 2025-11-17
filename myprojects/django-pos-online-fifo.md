#🏪 Django **"Sale Management System for a Pharmaceutical Shop"** .(FIFO Logic)

##📋 Description

A full-featured Django-based sale Management System that integrates POS (Point of Sale) and Online Ordering modules with FIFO stock logic, promotion control, and automated reporting.

---

This system is designed for pharmacy owners and customers, enabling:

Real-time inventory tracking (auto FIFO deduction)

POS order with instant invoice printing

Online order confirmation workflow (stock deduction only after confirmation)

Expiry & low-stock automatic alerts

Sales reporting with profit margin analytics

Chatbot for medicine & order inquiries

---

##🧠 Tech Stack

Backend: Django, Django REST Framework

Database: SQLite (development), PostgreSQL (production)

Auth: Django Auth + Email OTP

Frontend: TailwindCSS + Chart.js (Dashboard)

Stock Logic: FIFO-based multi-batch stock deduction

Deployment: Render / Railway / Localhost

---

#🚀 Core Features

##🧾 POS Module

Fast cashier-side sales entry (Cash / Mobile / Print)

Real-time stock deduction using FIFO batches

Automatic invoice generation + print preview

##🌐 Online Ordering Module

Customers browse medicines + active promotions

OTP-based registration & login

Orders reduce stock only when pharmacist confirms

Promotion logic auto-applies discounts

Expired promotions auto-cancel

📦 Inventory & Stock

Multi-batch FIFO management system

Auto stock sync when items are updated

Expiry tracking & alert notifications

📊 Reports & Dashboard

Filters: Daily / Weekly / Monthly / Yearly

POS vs Online comparison metrics

Revenue, transactions, items sold

Average profit margin analysis

Bar charts → Top 5 best-selling products (POS + Online)

🤖 Chatbot & Notifications

In-app chatbot for medicine & order-related queries

Customer dashboard notifications

Read / Unread toggle

"Mark all as read" feature included

---

##⚙️ How to Run (Development Setup)

# Clone the project
git clone https://github.com/kaunghtetsan/django-pos-online-fifo.git
cd django-pos-online-fifo

# Create virtual environment
python -m venv venv
venv\Scripts\activate       # On Windows
source venv/bin/activate    # On Mac/Linux

# Install dependencies
pip install -r requirements.txt

# Run migrations
python manage.py makemigrations
python manage.py migrate

# Create superuser (admin)
python manage.py createsuperuser

# Run server
python manage.py runserver

---

```markdown
![Dashboard](../assets/screenshots/pos_dashboard.png)